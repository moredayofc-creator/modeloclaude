---
name: video-quality-control
description: Audita vídeos educativos renderizados quanto a fatos, continuidade, sincronização, legibilidade e integridade técnica. Use antes de entregar qualquer MP4.
---

# Video Quality Control — Auditoria final

## Checklist editorial
- A pergunta central é respondida?
- A demonstração visual corresponde ao que a narração afirma?
- Números, datas e explicações estão verificados?
- O ritmo é adequado e não há frases cortadas?
- A conclusão é clara sem promessas enganosas?

## Checklist visual
- Personagem, figurino, proporções e materiais permanecem consistentes.
- Não há objetos atravessando superfícies, flicker, clipping, texturas quebradas ou câmera tremida acidental.
- Ação importante está visível e não fica escondida por texto.
- Legendas e rótulos estão dentro da área segura e são legíveis em celular.
- Não há frames pretos, frames congelados ou cenas ausentes sem intenção.

## Checklist de áudio
- Voz inteligível, sem clipping e sincronizada.
- Música não encobre a fala.
- Efeitos coincidem com as ações.
- Sem estalos, ruído inesperado ou cortes abruptos.

## Checklist técnico
- Confirme existência e tamanho do MP4.
- Use ffprobe para conferir duração, resolução, fps, codec de vídeo e áudio.
- Confirme que o vídeo pode ser decodificado integralmente.
- Confira início, meio, fim e transições com frames extraídos.
- Compare duração real com a solicitada; tolerância padrão de ±0,5 s, salvo pedido diferente.

## Relatório
Classifique cada achado como bloqueador, importante ou cosmético. Corrija bloqueadores e importantes antes da entrega. Se não for possível corrigir, informe explicitamente e não chame o vídeo de finalizado.
