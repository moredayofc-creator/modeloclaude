# 3D VIDEO STUDIO

Kit de Skills para Claude Code voltado à produção de vídeos educativos 3D.

## O que contém
- Diretor/orquestrador de produção.
- Roteiro educativo em português brasileiro.
- Storyboard técnico e continuidade visual.
- Construção de cenas 3D com Blender Python.
- Animação de personagens.
- Design e sincronização de áudio.
- Montagem/exportação com FFmpeg.
- Controle de qualidade editorial e técnico.

## Instalação
As Skills ficam em `.claude/skills/` e são descobertas automaticamente pelo Claude Code quando o repositório é aberto como projeto.

1. Clone ou atualize este repositório.
2. Abra a pasta no Claude Code.
3. Reinicie a sessão se as Skills não aparecerem imediatamente.
4. Digite `/3d-video-studio` para iniciar uma produção.
5. Use as Skills individuais: `/educational-script`, `/visual-storyboard`, `/blender-scene`, `/character-animation`, `/sound-design`, `/video-renderer` e `/video-quality-control`.

## Requisitos de produção
- Claude Code.
- Blender com suporte a Python/bpy para pipeline 3D.
- FFmpeg e ffprobe para montagem, áudio e validação.
- Espaço em disco para arquivos .blend, renders e masters.
- Voz/TTS ou gravação de narração; serviço externo é opcional e requer configuração própria.

O projeto verifica o ambiente antes de produzir. A ausência de uma ferramenta deve ser informada; nenhuma renderização é considerada concluída sem validação do MP4.

## Padrão
60 segundos, 1080×1920, 9:16, 30 fps, pt-BR, H.264/AAC, salvo instrução diferente.

## Importante
O pipeline não usa Remotion. Preserve o projeto web original e seus arquivos; o kit de Skills adiciona instruções e não substitui assets existentes.
