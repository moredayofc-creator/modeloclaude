---
name: video-renderer
description: Monta cenas, narração, efeitos, música e legendas e exporta vídeos MP4 verticais com FFmpeg. Use para finalizar e renderizar o vídeo.
---

# Video Renderer — Montagem e exportação

## Preparação
- Verifique a disponibilidade e versão do FFmpeg/ffprobe.
- Leia os metadados dos vídeos/áudios de entrada antes de montar.
- Normalize dimensões, fps, pixel format, timebase e sample rate.
- Preserve masters intermediários e não sobrescreva arquivos do usuário.

## Padrão de exportação
- MP4, H.264, yuv420p, 1080×1920, 30 fps, AAC 48 kHz estéreo.
- Use CRF 18–23 ou bitrate adequado ao material; preset equilibrado entre qualidade e tempo.
- Defina faststart para reprodução web.
- Sincronize áudio e vídeo por timestamps; trate duração final explicitamente.
- Legendas em SRT/ASS com safe margins, contraste e tamanho legível em celular.
- Não estique imagens nem distorça proporções; use crop/pad deliberado.

## Montagem
- Prefira concatenar cenas com parâmetros compatíveis ou use filter_complex quando houver transições.
- Aplique fades e transições com duração definida.
- Mixe voz, música e SFX em faixas controladas.
- Não use Remotion.
- Gere também um arquivo de legendas e um manifesto da montagem.

## Verificação
Use ffprobe para confirmar resolução, duração, fps, codecs e presença de áudio. Decodifique o arquivo inteiro quando possível para detectar corrupção. Extraia frames em pontos representativos e revise visualmente. Reproduza/analise o áudio final para verificar sincronização e clipping.

Nunca declare sucesso apenas porque o comando FFmpeg terminou sem erro: confira o arquivo gerado e seus metadados.
