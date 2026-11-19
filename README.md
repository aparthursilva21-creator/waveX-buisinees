# Pão Recheado · Conceito waveX com 3D + AR

Projeto demonstrativo **não oficial** da waveX para apresentar ao restaurante Pão Recheado Hamburgueria (Samambaia Norte, DF).

## Conteúdo
- Cardápio HTML responsivo, com navegação, busca e seleção ilustrativa sem envio de pedidos.
- Visualização 3D interativa (girar, aproximar) de quatro **modelos autorais ilustrativos**: Burger Tradicional, Burger Duplo, Combo Burger e Pão Recheado.
- Botão de realidade aumentada no celular **quando aparelho + navegador forem compatíveis**. Android usa WebXR/Scene Viewer; iPhone Safari pode usar Quick Look com conversão USDZ em tempo de execução. Depende de internet para carregar o componente externo model-viewer.
- Proposta comercial `proposta.html` e apresentação de QR Code/NFC. 

## Como publicar grátis no GitHub Pages
1. Entre em `https://github.com/new` e crie um repositório **público** chamado `wavex-pao-recheado-demo`, sem arquivos iniciais (ou com README, tanto faz).
2. Na aba **Add file → Upload files**, envie **os arquivos e pastas de dentro deste ZIP**, de modo que `index.html` fique **na raiz** do repositório. Não envie apenas o ZIP como arquivo.
3. Faça o commit das alterações.
4. Vá a **Settings → Pages → Build and deployment**. Em **Source**, escolha **Deploy from a branch**; em Branch selecione **main** e **/(root)**. Clique em Save.
5. O site tende a ficar em `https://SEU_USUARIO.github.io/wavex-pao-recheado-demo/`. Aguarde a confirmação no próprio GitHub.
6. Abra em um smartphone pelo HTTPS para testar **3D** e, se compatível, **AR**. Em desktop, o modelo 3D gira, mas não abre câmera.

## Realismo e autorização
Os GLBs são criações 3D estilizadas para demonstração. **Não são reconstruções dos lanches reais** nem devem ser apresentados ao restaurante como fotos fiéis. Para reprodução fiel de ingredientes e escala, a waveX precisa obter fotos, referências, medidas e autorização do proprietário; poderá contratar fotogrametria/modelagem 3D.

Não há checkout nem envio real de pedidos. Valores, composição e disponibilidade devem ser confirmados no cardápio oficial. Fotografias são externas e ilustrativas, podem falhar por bloqueio de rede. Este projeto deve ser apresentado como proposta não oficial, não como cardápio oficial da loja.

## Arquivos
- `index.html` — site demonstrativo com 3D/AR
- `proposta.html` — proposta comercial
- `assets/estilo.css` — estilos
- `assets/cardapio.js` — dados e interatividade
- `assets/modelos/*.glb` — modelos 3D autorais
- `assets/wavex-logo.png` — logo waveX
- `.nojekyll` — desabilita processamento Jekyll

## Tecnologias
HTML, CSS, JS, GLB/glTF e Google `<model-viewer>` distribuído por CDN.

## Observações comerciais
NFC é vendido separadamente; chip NFC armazena apenas URL; QR Code abre uma URL. Modelagem fiel e AR são adicionais opcionais com preço por complexidade, diferente do cardápio 2D.
