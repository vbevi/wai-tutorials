---
title: "Árvore de Decisão para Textos Alternativos"
title_html: "Arvore de Decisão para <code>alt</code>"
permalink: /tutorials/images/decision-tree/
ref: /tutorials/images/decision-tree-ptbr/
lang: pt-br
description:
image: /content-images/wai-tutorials/images/social.png
github:
  branch: 'master-2.0'
  repository: w3c/wai-tutorials
  path: 'content/images/decision-tree-ptbr.md'

resource:
  ref: /tutorials/images/
navigation:
  previous: /tutorials/images/imagemap/
  next: /tutorials/images/tips/

wcag_techniques:


metafooter: true
last_updated: 2023-05-12
editors:
  - Eric Eggert: "https://www.w3.org/People/yatil/"
  - Shadi Abou-Zahra: "https://www.w3.org/People/shadi/"
update_editors:
  - Brian Elton
contributors:
  - veja <a href="/WAI/tutorials/acknowledgements/">Acknowledgements</a>
suporte: Desenvolvido pelo Education and Outreach Working Group (<a href="https://www.w3.org/groups/wg/eowg">EOWG</a>). Criado com o suporte do <a href="https://www.w3.org/WAI/ACT/">WAI-ACT project</a>, co-fundado pelo <strong>Programa <abbr title="Information Society Technologies">IST</abbr> da Comissão Européia</strong>.
---

{::nomarkdown}
{% include box.html type="start" h="2" title="Overview" class="full" %}
{:/}

Esta árvore de decisão descreve como usar o atributo `alt` em elementos <img> em diversas situações. Para diferentes tipos de imagens podem ser usadas abordagens diferentes, como usando imagens de fundo CSS para imagens decorativas ou web fonts ao invés de imagens contendo só textos.

{::nomarkdown}
{% include box.html type="end" %}
{:/}

- **A imagem contém texto?**
  - {:.yes} **Sim:**
    -   **… e o mesmo texto também está presente e próximo como um texto *real*.**
      _Use o atributo `alt` vazio. Veja [Decorative Images](/tutorials/images/decorative/) (em Inglês)._
    -   **… e o texto é somente um efeito visual.**
      _Use o atributo `alt` vazio. Veja [Decorative Images](/tutorials/images/decorative/) (em Inglês)._
    -   **… e o texto tem uma função específica, como por exemplo ser um ícone.**
      _Use o atributo `alt` para comunicar a função da imagem. Veja [Functional Images](/tutorials/images/functional/) (em Inglês)._
    -   **… e o texto na imagem não estaria presente de outra forma.** _Use o atributo `alt` para incluir o texto da imagem. Veja [Images of Text](/tutorials/images/textual/#image-of-styled-text-with-decorative-effect) (em Inglês)._
  - {:.no} **Não:**
    - Continue.
- **A imagem é usada em um link ou botão, e seria difícil ou impossível entender o que tal link/botão faz caso a imagem não estivesse ali?**
  - {:.yes} **Sim:**
    -  _Use o atributo `alt` para comunicar a página de destino do link ou a ação que o botão iniciará. Veja [Functional Images](/tutorials/images/functional/) (em Inglês)._
  - {:.no} **Não:**
    - Continue.
- **A imagem contribui para o entendimento da página ou seu contexto?**
  - {:.yes} **Sim:**
    - **… e é um elemento visual simples ou uma foto.**
      _Use uma descrição curta da imagem para descrever qual contexto ou significado ela transmite no atributo `alt`. Veja [Informative Images](/tutorials/images/informative/)(em Inglês)._
    - **… e é um gráfico ou um elemento visual complexo.**
      _Inclua a informação continda na imagem em outro lugar na página. Veja [Complex Images](/tutorials/images/complex/) (em Inglês)._
    - **… e ela mostra conteúdo que é redundante com algum texto *real* que esteja próximo dela.**
      _Use o atributo `alt` vazio. Veja (redundant) [Functional Images](/tutorials/images/functional/#logo-image-within-link-text)(em Inglês)._
  - {:.no} **Não:**
    - Continue.
- **A imagem é meramente decorativa ou não destinada ao usuário?**
  - {:.yes} **Sim:**
    - _Use o atributo `alt` vazio. Veja [Decorative Images](/tutorials/images/decorative/) (em Inglês)._
  - {:.no} **Não:**
    - Continue.
- **O tipo de uso da imagem não está contemplado acima ou não é claro qual `alt` fornecer?**
  - {:.yes} Esta árvore de decisão **não contempla** todos os casos. Para informações mais detalhadas no fornecimento de textos alternativos, confira a página [Image Concepts Page](/tutorials/images/) (em Inglês).
{:.decision-tree}
