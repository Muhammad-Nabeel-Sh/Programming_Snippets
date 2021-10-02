# Libraries, Frameworks and API's

## Bootstrap and Fontawesome

```HTML
<!-- Bootstrap CSS Framework -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/5.1.1/css/bootstrap.min.css" integrity="sha512-6KY5s6UI5J7SVYuZB4S/CZMyPylqyyNZco376NM2Z8Sb8OxEdp02e1jkKk/wZxIEmjQ6DRCEBhni+gpr9c4tvA==" crossorigin="anonymous" referrerpolicy="no-referrer" />

<!-- Fontawesome CSS Framework -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css" integrity="sha512-1ycn6IcaQQ40/MKBW2W4Rhis/DbILU74C1vSrLJxCq57o941Ym01SwNsOMqvEBFlcgUa6xLiPY/NS5R+E6ztJQ==" crossorigin="anonymous" referrerpolicy="no-referrer" />
```

## highlight.js

```HTML
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.2.0/styles/atom-one-dark.min.css" integrity="sha512-Jk4AqjWsdSzSWCSuQTfYRIF84Rq/eV0G2+tu07byYwHcbTGfdmLrHjUSwvzp5HvbiqK4ibmNwdcG49Y5RGYPTg==" crossorigin="anonymous" referrerpolicy="no-referrer" />

<script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.2.0/highlight.min.js" integrity="sha512-MinqHeqca99q5bWxFNQEQpplMBFiUNrEwuuDj2rCSh1DgeeTXUgvgYIHZ1puBS9IKBkdfLMSk/ZWVDasa3Y/2A==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
```

```js
function highlightCode() {
    var pres = document.querySelectorAll("pre>code");
    for (var i = 0; i < pres.length; i++) {
        hljs.highlightBlock(pres[i]);
    }
}
highlightCode();
```

## MathJax Framework for LaTeX typesetting

```HTML
<script src="https://polyfill.io/v3/polyfill.min.js?features=es6"></script>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
```

## KaTeX -- The fastest math typesetting library for the web.

```HTML
 <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@0.13.18/dist/katex.min.css" integrity="sha384-zTROYFVGOfTw7JV7KUu8udsvW2fx4lWOsCEDqhBreBwlHI4ioVRtmIvEThzJHGET" crossorigin="anonymous">

<!-- The loading of KaTeX is deferred to speed up page rendering -->
<script defer src="https://cdn.jsdelivr.net/npm/katex@0.13.18/dist/katex.min.js" integrity="sha384-GxNFqL3r9uRJQhR+47eDxuPoNE7yLftQM8LcxzgS4HT73tp970WS/wV5p8UzCOmb" crossorigin="anonymous"></script>

<!-- To automatically render math in text elements, include the auto-render extension: -->
<script defer src="https://cdn.jsdelivr.net/npm/katex@0.13.18/dist/contrib/auto-render.min.js" integrity="sha384-vZTG03m+2yp6N6BNi5iM4rW4oIwk5DfcNdFfxkk9ZWpDriOkXX8voJBFrAO7MpVl" crossorigin="anonymous" onload="renderMathInElement(document.body);"></script>

<!-- You can prefetch KaTeX fonts to prevent FOUT or FOIT. -->
<script>
  window.WebFontConfig = {
    custom: {
      families: ['KaTeX_AMS', 'KaTeX_Caligraphic:n4,n7',   'KaTeX_Fraktur:n4,n7',
                'KaTeX_Main:n4,n7,i4,i7', 'KaTeX_Math:i4,i7', 'KaTeX_Script',
                'KaTeX_SansSerif:n4,n7,i4', 'KaTeX_Size1', 'KaTeX_Size2', 'KaTeX_Size3',
                'KaTeX_Size4', 'KaTeX_Typewriter'],
    },
  };
</script>
<script defer src="https://cdn.jsdelivr.net/npm/webfontloader@1.6.28/webfontloader.js" integrity="sha256-4O4pS1SH31ZqrSO2A/2QJTVjTPqVe+jnYgOWUVr7EEc=" crossorigin="anonymous"></script>
```

## Animate on Scroll Library

```HTML
<link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
<script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
```

```js
AOS.init();
```

## DJ3

```HTML
<script src="https://cdnjs.cloudflare.com/ajax/libs/d3/7.0.1/d3.js" integrity="sha512-GtmGlfEaLcFKLAK57uct3sNffu1QPAu1/KxdPOieXEz1tgQS5BcU7GQuYKlzYUrgZmeEGjuE1Mgvdi1241bh6A==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
```

## Chart.js

```HTML
<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/3.5.1/chart.js" integrity="sha512-b3xr4frvDIeyC3gqR1/iOi6T+m3pLlQyXNuvn5FiRrrKiMUJK3du2QqZbCywH6JxS5EOfW0DY0M6WwdXFbCBLQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
```

## Anime.js

```HTML
<script src="https://cdnjs.cloudflare.com/ajax/libs/animejs/3.2.1/anime.js" integrity="sha512-E378bwaeZf1nwXeJGIwTB58A5gPt5jFU3u6aTGja4ZdRFJeo/N/REKnBgNZOZlH6JdnOPO98vg2AnSGaNfCMFQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
```