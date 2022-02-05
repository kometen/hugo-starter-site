---
title: "Blogge Med Hugo"
date: 2022-01-30T19:23:45+01:00
draft: false
---
#### Hvad er Hugo?

[Hugo](https://gohugo.io/) er et værktøj til at lave websider hvor du kan publicere artikler, tanker, idéer, eller hvad som ellers ligger dig på sinde. Der findes mange temaer du kan lægge oven på, så din webside vises på den måde du ønsker.

Mange alternativer tilbyder noget tilsvarende. Wordpress og Squarespace er to eksempler. Disse er meget fleksible, men medfører også lidt administration. Her foregår arbejdet med websiden via en netlæser på en server hos de der leverer tjenesten.

Med Hugo oprettes websiden på din mac/pc, og artiklerne skrives i formatet [Markdown](https://en.wikipedia.org/wiki/Markdown). Teksten oversættes dernæst til HTML. En beskrivelse af formatet findes [her](https://www.markdownguide.org/basic-syntax/).

Dernæst skal indholdet lægges på en server som er tilgængelig på internettet. [Cloudflare](https://www.cloudflare.com) tilbyder en sådan tjeneste. Cloudflare er en vigtig del af interenttets infrastruktur, hvor de sørger for at indhold sendes frem så hurtig som mulig, beskytter websider som er under angreb med mere.

Hugo er mere rettet mod webudviklere, og denne metode er mere manuel end med Wordpress, Squarespace eller tilsvarende. Men til enkle formål kan Hugo erstatte disse værktøjer.

Det eksempel jeg viser her bruger [Cloudflare Pages](https://pages.cloudflare.com). Websiden sendes dog ikke direkte til Cloudflare, men går via [GitHub](https://github.com) eller [GitLab](https://about.gitlab.com) før det kan vises. Det koster ikke noget at oprette en konto på disse tre tjenester, så websiden kan laves uden at det koster penge.

GitHub og GitLab er virksomheder som du kan laste din kode op til, skrevet i kodeversioneringsværktøjet Git. Koden kan så gøres offentlig så andre kan se den, eller gøres privat, hvis du ikke ønsker andre skal se.

Jeg har brugt macos, men Linux, Windows, *BSD er gode alternativer. Det enkleste er hvis du åbner et terminalvindue. På macos kan programmet `Terminal` benyttes.

#### Hvordan installére Hugo?

##### Installér programmet Hugo
[Homebrew](https://brew.sh/) er et program som kan installere programmer på macos. Andre operativsystemer har tilsvarende alternativer.

`brew install hugo`

##### Opret en webside med

`hugo new site hugo-starter-site`

##### Gå ned i mappen

`cd hugo-starter-site`

##### Klargør for versionerings-værktøjet git

`git init`

Git bruges for at huske ændringer der laves i kode, samt at hente temaer (skins). Der findes mange temaer som findes på https://themes.gohugo.io/. Jeg har valgt temaet Anatole som kan ses på https://themes.gohugo.io/themes/anatole/.

##### Temaet installeres med

`git submodule add https://github.com/lxndrblz/anatole.git themes/anatole`

##### Lav den første artikel med

`hugo new posts/hej-med-dig.md`


### Alt tekst under dette punkt er notater jeg har skrevet undervejs, og kan dels være mangelfulde, selvmodsigende, da jeg lærte mens jeg fejlsøgte. Jeg vil rydde i dette, og håbet er at andre kan lave noget tilsvarende. Jeg brugte bla. en del tid på at lægge mulighed for at vælge mellem dansk og engelsk ind sprog ind.

##### Åben content/posts/hej-med-dig.md i en editor og skriv noget nederst, f.eks.

`Dette er min første artikel skrevet med Hugo.`

##### Læg alle filer i git-værktøjet

`git add .`

##### Registrer al ny kode med

`git commit -am "Min første artikel"`

##### Læg koden ud på github med

`gh repo create`
