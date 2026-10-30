---
name: blender-scene
description: Cria cenas 3D educativas no Blender usando Python e bpy, incluindo geometria, materiais, iluminação, câmeras e animação. Use para construir ou renderizar cenas 3D.
---

# Blender Scene Builder

## Antes de criar
1. Verifique se Blender está instalado e capture a versão.
2. Leia a documentação da API compatível com a versão instalada; não invente propriedades ou operadores.
3. Inspecione assets existentes e reutilize-os quando possível.
4. Defina unidades, escala, fps, resolução, engine e color management explicitamente.

## Construção
- Escreva scripts Python reproduzíveis usando bpy; salve o .blend e o script fonte.
- Organize objetos em collections com nomes claros (CHARACTER, ENVIRONMENT, PROPS, LIGHTS, CAMERAS, FX).
- Use materiais nomeados e parâmetros centralizados; evite valores mágicos espalhados.
- Crie iluminação de três pontos quando apropriado, com luz de recorte e sombras controladas.
- Configure câmera vertical 9:16 e confira safe areas.
- Anime propriedades com keyframes, curvas e easing; use constraints/rigs quando necessário.
- Para explicações técnicas, use cortes, peças separadas, transparência e animação de montagem/desmontagem.
- Faça render de teste de baixa amostragem antes do render final.
- Renderize cenas por intervalos ou arquivos separados quando isso facilitar correções.

## Qualidade e desempenho
- Evite geometria desnecessária, subdivisões excessivas e texturas enormes.
- Use denoise quando adequado e teste flicker, sombras, transparências e motion blur.
- Garanta que a cena tenha câmera ativa, iluminação, world, frame range e output configurados.
- Verifique os logs de execução e confirme que os arquivos de render foram realmente escritos.

## Fallback
Se Blender não estiver instalado, não finja que criou 3D. Informe o bloqueio e proponha instalação/configuração ou uma alternativa já presente no projeto, como Three.js/WebGL, mantendo a natureza tridimensional.

## Entrega
Salvar .blend, .py, renders de teste e render final/intermediário em pasta de projeto organizada. Registrar versão do Blender e configurações usadas.
