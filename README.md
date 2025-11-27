Undertale Mini Wiki — README
Visão geral

Undertale Mini Wiki é uma página web de uma única página (index.html) que apresenta uma mini wikipédia do universo de Undertale. É uma página web simples em HTML feita para hospedagem temporária

Funcionalidades principais

Tema escuro com contraste alto (legibilidade em foco).

Cabeçalho com logo e banner de destaque.

Seções: Home, História (vídeo incorporado) e Personagens.

Grid responsivo com as caixas de personagens.

Imagens clicáveis que revelam/ocultam descrições (comportamento controlado por JavaScript simples).

Layout responsivo básico para dispositivos móveis.

Estrutura do arquivo

O projeto consiste apenas de:

index.html

Todo o HTML, CSS e JavaScript estão embutidos dentro desse arquivo.

Como usar

Baixe (ou copie) o arquivo index.html.

Abra-o diretamente no navegador (Chrome, Firefox, Edge, Safari).

Para editar texto, imagens ou estilos, abra index.html num editor de texto (VSCode, Sublime, Notepad++ etc.), faça as alterações e salve.

Recarregue a página no navegador para ver as mudanças.

Principais trechos editáveis

Cabeçalho: logo e estilos em header (linha no topo do arquivo).

Banner: imagem com classe banner.

Seções: blocos <section id="home">, <section id="historia">, <section id="personagens">.

Personagens: cada personagem é um bloco .perso-box contendo <h3>, <img> com onclick e <div id="iX"> com o texto.

CSS: dentro da tag <style> no <head> (cores, tamanhos, responsividade).

Script: função toggleConteudo(id) embutida na seção de personagens (para abrir/fechar descrições).

Como modificar ou estender

Adicionar/remover personagem: copie um bloco .perso-box e atualize h3, src da imagem e o id do div de descrição (i1 → i11 etc.), e a chamada onclick="toggleConteudo('iX')" correspondente.

Alterar cores: edite as variáveis/valores no CSS (por exemplo border: 2px solid #913b85; e border-top: 3px solid #5e2356;).

Separar CSS/JS externos: mova o conteúdo de <style> para style.css e a função toggleConteudo para script.js, e referencie com <link> / <script src=>.

Accordion (fechar um ao abrir outro): substituir a função toggleConteudo por uma que feche todas antes de abrir a selecionada (exemplo disponível na documentação técnica).

Acessibilidade e recomendações

alt em imagens: já presentes; mantenha textos descritivos para leitores de tela.

Contraste: tema escuro já utiliza contraste; verifique WCAG se for necessário conformidade.

Navegação por teclado: imagens com onclick não são focáveis por padrão — considere trocar por <button> ou adicionar tabindex="0" e keydown handlers para acessibilidade.

Licença e créditos

Este projeto é um fan-made e educativo.

Undertale é propriedade de Toby Fox.

Use o projeto para aprendizado e demonstração; não comercialize materiais protegidos por direitos autorais sem permissão.
