# Criando-Pagina-de-Portifolio

## Um passo a passo detalhado de como criar uma landing page do zero utilizando HTML e CSS. A transcrição utilizada como base aborda a criação de uma página com diferentes seções, incluindo cabeçalho, área de boas-vindas, call-to-actions, portfólio, serviços e rodapé.

Serão explicados conceitos importantes como:


Estrutura básica de um documento HTML
Utilização de tags semânticas
Estilização dos elementos com CSS
Uso de classes e IDs
Técnicas de layout com Flexbox
Boas práticas de código

```
Entender a estrutura básica de uma página HTML
Utilizar tags HTML de forma semântica
Aplicar estilos CSS aos elementos
Posicionar elementos na página com Flexbox
Organizar o código de forma limpa e eficiente

Vamos começar!

Estrutura Básica do HTML

A linguagem de marcação HTML é utilizada para estruturar o conteúdo de sites e páginas na web. Todo documento HTML possui uma estrutura básica que deve ser seguida:

<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<title>Título da Página</title>
</head>
<body>
<h1>Título Principal</h1>
<p>Conteúdo da página...</p>
</body>
</html>


Analisando o código acima, temos:


<!DOCTYPE html>: Declaração do tipo de documento, no caso HTML5. É obrigatória.
<html>: Tag raiz de um documento HTML. Todo o conteúdo deve estar dentro dela.
<head>: Cabeçalho do documento. Contém meta informações e configurações.
<title>: Define o título da página que aparece na aba do navegador.
<body>: Corpo do documento onde está todo o conteúdo visível.
<h1>: Título de nível 1.
<p>: Parágrafo de texto.

Essa é a estrutura básica de qualquer página HTML. A partir dela podemos começar a adicionar os componentes da nossa landing page.

Criando o Header

O cabeçalho (header) geralmente contém elementos como logo, menu de navegação e botões de ação (call-to-actions). Vamos criá-lo utilizando a tag <header>. Dentro dela adicionaremos:


Um título <h1> com o nome ou logo da empresa
Uma navegação <nav> com links internos
Um botão de ação primário

A estrutura ficará assim:

<body>

<header>

<h1>Nome da Empresa</h1>

<nav>
<a href="#services">Serviços</a>
<a href="#about">Sobre</a>
<a href="#contact">Contato</a>
</nav>

<a href="#" class="btn">Fale Conosco</a>

</header>

</body>


Repare que estamos utilizando tags semânticas como <header>, <nav> e <a> para links. Isso ajuda na estrutura e significado do código.

Também adicionamos uma classe btn no botão de ação para poder estilizá-lo depois com CSS.

Estilizando com CSS

Agora que temos a estrutura do header em HTML, podemos começar a estilizar os elementos com CSS. O CSS é responsável pela aparência visual do site.

Vamos criar um arquivo style.css e importá-lo no HTML:

<head>
<link rel="stylesheet" href="style.css">
</head>


Depois podemos começar a aplicar estilos. Por exemplo, centralizar o menu de navegação:

nav {
display: flex;
justify-content: center;
}


E estilizar o botão primário:

```css

.btn {
padding: 1em 2em;
border: none;
border-radius: 5px;
background: #007bff;
color: #fff;
}

Perceba que todo seletor CSS deve fazer referência a uma classe ou tag HTML. Assim conseguimos vincular os estilos.

## Área de Boas Vindas

Abaixo do cabeçalho, páginas de conversão geralmente possuem uma área de boas vindas, saudação e valor proposta. Esta seção pode conter:

- Um título de impacto (tag H2)
- Um subtítulo ou saudação
- Um parágrafo de texto introdutório
- Um botão de ação secundário

Ficaria assim:


html



Título de impacto


Saudação



Texto introdutório...


Botão secundário


Repare que usamos uma tag `<section>` para agrupar o conteúdo, e um ID #about para identificar esta seção e poder linkar o menu de navegação.

O botão secundário também possui uma classe específica para ser estilizada de forma diferente.

## Call to Actions

Call-to-actions (CTAs) são elementos de convite/chamada para uma ação específica.

Geralmente são botões ou links proeminentes que incentivam o visitante a fazer algo como: cadastre-se, inscreva-se, compre agora.

Podemos criar uma seção de CTAs com 3 colunas, cada uma com:

- Um ícone
- Um título (h3)
- Um texto resumido

Ficaria assim:


html





Título CTA 1


Descrição curta e convincente do CTA 1












Foram utilizadas classes e IDs para identificar as seções, e divs para agrupar cada coluna, tornando fácil a estilização com CSS depois.

## Criando uma Galeria de Projetos

Para mostrar projetos já realizados, podemos criar uma galeria com Flexbox:


html



Portfólio









E então definir no CSS que a div gallery terá display flex, para posicionar as imagens lado a lado horizontalmente.

Assim construímos uma galeria responsiva de forma fácil com flexbox e CSS.

## Listando Serviços

Para exibir os serviços oferecidos pela empresa, podemos fazer uma seção contendo:

- Título da seção (h2)
- Título dos serviços (h3)
- Descrição curta de cada serviço (parágrafos)
- Ícones representativos

Ficaria assim:


html



Serviços




Consultoria


Consultoria especializada...





Email Marketing


Email marketing eficiente...




Repare que usamos classes e IDs para identificar as seções, e divs para agrupar e organizar os serviços.

Isso facilita a estilização e manutenção futura.

## Criando um Rodapé

O rodapé geralmente contém informações secundárias como dados de contato, informações legais, links úteis e mapa do site.

Podemos criar um rodapé com:

- Logo e dados de contato
- Menu secundário de links úteis
- Selos de certificações
- Copyright ou informações legais

Assim finalizamos a estrutura HTML da nossa landing page. Agora é só estilizar os elementos com CSS!

Considerações Finais

Neste ebook você aprendeu na prática como estruturar uma landing page completa apenas com HTML e CSS.

Vimos como organizar o conteúdo em seções semânticas, utilizando as tags corretas para cada elemento. Também aplicamos estilos e posicionamos os componentes com flexbox.

Dominar essas técnicas é essencial para qualquer desenvolvedor front-end. Você pode utilizar este conhecimento como base para criar diversos tipos de sites e páginas responsivas.

E lembre-se de sempre manter um código limpo, organizado e fácil de dar manutenção. Isso fará toda diferença nos seus projetos.

Agora é só colocar a mão na massa e praticar!
