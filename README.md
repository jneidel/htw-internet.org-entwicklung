# htw-internet.org-entwicklung

> Wie entwickelte sich Facebooks Internet.org/Free Basics in Indien? - Wissenschaftliche Arbeit an der HTW Berlin in Gesellschaftliche Aspekte der Informatik (B15GesAsp)

[Arbeit als PDF](main.pdf).

## Einleitung

Die folgende Arbeit beschäftigt sich mit der Entwicklung von Facebooks 'Internet.org' in Indien. Die Initiative möchte das Internet zu den Menschen bringen, denen das Internet sonst unzugänglich bleiben würde.


Indien hat, als eins der bevölkerungsreichsten Länder der Erde mit einer Gesellschaft, die langsam an das Internet angeschlossen wird, enormes wirtschaftliches Potential,
wovon Facebook, mit seinen schwächelnden Nutzerwachstumsumszahlen, gern profitieren möchte.
Um neue Nutzer für die Platform zu gewinnen, soll die Internet.org Initiative genutzt werden, um das Internet zu den bisher unangebundenen Menschen zu bringen.
In seinem ambitionierten Konzept spricht Mark Zuckerberg davon, Menschen durch die Anbindung an globale Märkte, das Wissen der Welt und den Rest der Menschheit aus der Armut zu entheben.


Wir möchten der Umsetzung von Internet.org auf den auf den Grunde gehen, um zu erfahren, ob Zuckerberg die Umsetzung seines Versprechens geglückt ist.

Im Zuge dessen beleuchten wir zunächst die Ausgangssitionation: von den Gegebenheiten Indiens (Facebooks Bedeutung in der Bevölkerung, der Umgang mit dem Internet generell, vorherige Begegnungen mit der Netzneutralitätsthematik) zu einer Ausführung von Facebooks Konzept für Internet.org.

Nach Verständnis der Ausgangslage werden die verschiedenen Zeitabschnitte, von der Einführung bis zum Verbot, die Reaktionen der Bevölkerung, sowie die Erfüllung des umschriebenen Nutzens betrachtet.

## Build

Run `./build`

**Dependencies**

`yay -S texlive-core texlive-bibtexextra biber`

## Style guide

### Citations

```tex
% given this source in bibliography:
% @book{twoBits,
%   author = {Christopher M. Kelty},
%   date = {2008},
%   title = {Two Bits: the Cultural Significance of Free Software},
% }


\textcite{twoBits} % => Christopher M. Kelty (2008)
% use in text

\cite{twoBits} % => Christopher M. Kelty 2008
\cite[28]{twoBits} % => Christopher M. Kelty 2008, p. 28
% use after direct quote

\parencite{twoBits} % => (Christopher M. Kelty 2008)
\parencite[Vgl.][28]{twoBits} % => (Vgl. Christopher M. Kelty 2008, p. 28)
% use at the end of text

\autocite{twoBits} % => ^1 (squared one, and a footnote with normal \cite)
% use if would be too big (webpages)
```

see: [biber introduction](https://en.wikibooks.org/wiki/LaTeX/Bibliographies_with_biblatex_and_biber)

### Quotes

```tex
% citations with corret quotes:
``this is a quote" or a `specific phrase'
% instead of the wrong "this is a quote" or a 'specific phrase'
```

Output of wrong quotes: ![](https://i.imgur.com/NZOdoiG.png)

Output of correct quotes: ![](https://i.imgur.com/rkB7vLH.png)

### Text breaks

To separate two blocks of text use `\medskip`.

### Sections

There are different level of sections:
- `\section` is the top level section (e.g. 2.)
- `\subsection` is a nested section (e.g. 2.1.)
- `\subsubsection` is a nested a level deeper (e.g. 2.1.3.)
- etc.

