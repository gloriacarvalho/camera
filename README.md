# Foto ON-lline — Estúdio de Captura

Aplicação web para acessar a câmera do dispositivo, capturar uma fotografia, aplicar um efeito visual e gravar identificação, data e hora diretamente na imagem.

## Integrantes
- Glória Maria Moura Bruno De Carvalho

## Tecnologias e recursos
- HTML5 para a estrutura da página.
- CSS3 para a interface responsiva.
- JavaScript para eventos, manipulação do DOM e tratamento de situações.
- `navigator.mediaDevices.getUserMedia()` para solicitar acesso à câmera.
- `Canvas` (`getContext`, `drawImage`, `filter`, `fillText` e `toBlob`) para processar a imagem.
- `MediaStreamTrack.stop()` para encerrar corretamente as faixas da câmera.

## Funcionalidades
- Iniciar e desligar a câmera.
- Exibir a câmera em tempo real.
- Capturar uma fotografia.
- Aplicar efeito original, preto e branco, sépia ou alto contraste.
- Gravar identificação, data e hora na própria imagem.
- Visualizar e baixar a imagem final em PNG.
- Orientar o usuário em casos de permissão negada, ausência de câmera ou indisponibilidade do dispositivo.

## Como executar
1. Abra a pasta no Visual Studio Code.
2. Inicie a página com a extensão Live Server.
3. Permita o acesso à câmera quando o navegador solicitar.
4. Digite uma identificação, selecione um efeito e clique em **Capturar foto**.

> O acesso à câmera exige um contexto seguro, como `localhost` (Live Server) ou HTTPS. Se a permissão for negada, altere a permissão do site nas configurações do navegador e tente novamente.

## Requisito de privacidade
A imagem é processada no navegador e não é enviada a um servidor. O acesso à câmera é encerrado ao clicar em “Desligar câmera” e quando a página é fechada ou abandonada.
