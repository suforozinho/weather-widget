# weather-widget
Um simples ferramenta para mostrar informações sobre o clima, usando custom elements e web components

## Instalação
Primeiro, na pasta Server, rode `npm install`. Depois na pasta root do projeto rode `npm install` também.
Na pasta Server, você precisa criar um `.env` com as suas keys do Google Maps e do DarkSky(https://darksky.net/dev), e na pasta root, você precisa criar também de um `.env` de acordo como está no exemplo.
Depois de todos esses preparativos, rode `npm start` na pasta Server, e na pasta root, `npm run watch`.

## Como usar
O tag do elemento é `<x-weather>` e ele tem dois paramêtros: `latitude` e `longitude`; o que ele irá mostrar dependerá dos valores que tem nesses atributos.
Para você editar o HTML dele, você terá que ir no arquivo `Weather.js` e editar o `innerHTML` dele. Como eu coloquei um shadow DOM no elemento, os estilos que tiver nele(aqueles do `innerHTML`) não afetarão o resto do HTML.
No arquivo `home.js` já tem um pequeno exemplo da funcionalidade dele.
