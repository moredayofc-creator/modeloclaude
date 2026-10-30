# Instruções do projeto — 3D VIDEO STUDIO

Este repositório está evoluindo de uma animação web minimalista para um estúdio de produção de vídeos educativos 3D. Preserve o projeto existente: não remova nem reescreva `index.html` sem pedido explícito.

## Objetivo padrão
Produzir vídeos educativos em português brasileiro, normalmente com 60 segundos, formato vertical 9:16, 1080×1920 e 30 fps (ou 24 fps quando solicitado). O resultado final deve ser um MP4 validado, não apenas um roteiro ou uma prévia.

## Regras de produção
- Antes de alterar arquivos, inspecione a estrutura, dependências, scripts, ambiente e recursos já existentes.
- Não presuma que Blender, FFmpeg, Python, codecs, fontes, modelos 3D ou serviços de voz estejam instalados. Verifique e explique bloqueios.
- Não use Remotion. Priorize Blender via Python para cenas 3D e FFmpeg para montagem, áudio, legendas e exportação. Use a tecnologia já adotada pelo projeto quando ela for claramente mais adequada.
- Não substitua animação 3D por imagens estáticas com zoom. Se uma cena exigir 3D, crie geometria, materiais, iluminação, câmera e animação reais ou declare claramente qualquer limitação.
- Preserve a continuidade visual: personagem, proporções, roupa, materiais, paleta, iluminação e escala devem permanecer consistentes entre cenas.
- Conteúdo educativo precisa ser correto, compreensível e demonstrado visualmente. Não invente números, mecanismos, dados ou alegações. Sinalize fatos que exigem verificação.
- Narração sempre em pt-BR, com texto natural, frases curtas e ritmo compatível com o tempo de cada cena.
- Sincronize ações, narração, legendas e efeitos sonoros usando timestamps explícitos.
- Gere arquivos intermediários organizados por projeto; nunca sobrescreva entregas anteriores sem autorização.
- Ao final, execute validações técnicas e informe caminho do MP4, resolução, duração, fps, áudio e eventuais limitações.

## Skills do projeto
Use as Skills em `.claude/skills/`:
- `/3d-video-studio`: coordena a produção completa.
- `/educational-script`: roteiro didático e narração.
- `/visual-storyboard`: cenas, planos e continuidade.
- `/blender-scene`: construção de cenas 3D.
- `/character-animation`: personagem, rig e atuação.
- `/sound-design`: voz, música e efeitos sincronizados.
- `/video-renderer`: montagem e exportação MP4.
- `/video-quality-control`: inspeção e validação final.

## Segurança e integridade
- Não execute comandos destrutivos ou remova arquivos sem autorização.
- Não faça upload de assets protegidos por direitos autorais sem licença.
- Nunca exponha chaves, tokens ou credenciais.
- Antes de instalar dependências, apresente o que será instalado e prefira ferramentas gratuitas/open-source quando possível.
