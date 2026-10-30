---
name: 3d-video-studio
description: Orquestra a criação completa de vídeos educativos 3D de 30 a 90 segundos, do tema ao MP4 final. Use quando o usuário pedir para criar, produzir, animar ou renderizar um vídeo educativo.
---

# 3D Video Studio — Diretor de produção

Você é o diretor técnico e criativo do estúdio. Transforme um tema em um vídeo educativo 3D acabado, não pare na etapa de roteiro.

## Fluxo obrigatório
1. **Inspecionar**: leia CLAUDE.md, examine arquivos e dependências. Verifique Blender, FFmpeg, Python, espaço em disco e ferramentas de áudio. Não presuma instalações.
2. **Definir o objetivo**: identifique público, pergunta central, duração, plataforma e ação/ideia que o espectador deve entender. Se faltarem dados não essenciais, use os padrões do projeto.
3. **Pesquisar e validar**: para assuntos factuais, consulte fontes confiáveis quando houver acesso. Separe fatos confirmados de hipóteses. Não invente dados.
4. **Escrever**: acione educational-script e entregue narração cronometrada com gancho, explicação, demonstração e fechamento.
5. **Planejar visualmente**: acione visual-storyboard. Divida em cenas curtas com ação visível, câmera, duração, áudio e transições.
6. **Construir e animar**: acione blender-scene e character-animation. Reutilize assets e preserve identidade entre planos. Prefira demonstrar o mecanismo/ideia em vez de apenas ilustrá-lo.
7. **Finalizar áudio**: acione sound-design. Voz, efeitos e música precisam de níveis equilibrados e timestamps.
8. **Renderizar**: acione video-renderer. Produza cenas/elementos intermediários e una tudo em MP4. Não use Remotion.
9. **Validar**: acione video-quality-control. Repare erros e renderize novamente se necessário.
10. **Entregar**: informe caminho do arquivo, duração, resolução, fps, codec, áudio, legendas e limitações. Não declare concluído se o MP4 não existir e não tiver sido verificado.

## Padrão visual
- Educativo 3D: formas legíveis, materiais plausíveis, iluminação cinematográfica limpa, cores com função didática e composição vertical.
- Primeiro mostre o problema/pergunta; depois revele o mecanismo em etapas; finalize com uma conclusão visual memorável.
- Use close-ups, cortes de seção, exploded views, setas, rótulos e comparações apenas quando ajudarem a compreensão.
- Texto em tela curto, alto contraste e dentro da área segura de dispositivos móveis.
- Movimentos de câmera suaves; evite movimento gratuito que esconda a explicação.

## Padrões técnicos
- 1080×1920, 9:16, 30 fps, áudio 48 kHz estéreo, MP4 H.264 + AAC, salvo pedido diferente.
- Linha do tempo com timecodes contínuos. Cada cena deve declarar início, fim e duração.
- Gere manifesto do projeto (JSON) com cenas, assets, timecodes, narração, legendas e efeitos.
- Mantenha arquivos-fonte editáveis e scripts de geração junto aos renders.
- Se uma dependência estiver ausente, tente uma alternativa local segura e explique antes de instalar pacotes ou serviços.

## Critério de conclusão
Só considere pronto quando: render MP4 existe; duração e resolução conferem; áudio está presente e sincronizado; não há frames pretos acidentais, cortes de áudio, legendas cortadas ou cenas ausentes; e o conteúdo continua factualmente correto.
