---
title: "Blogge Med Hugo"
date: 2022-01-30T19:23:45+01:00
draft: false
---

[Hugo](https://gohugo.io/) er et værktøj til at lave websider hvor du kan publicere artikler, tanker, idéer, eller hvad som ellers ligger dig på sinde. Der findes mange temaer du kan lægge oven på, så din webside vises på den måde du ønsker.

Der findes mange alternativer som tilbyder noget tilsvarende. Wordpress og Squarespace er to eksempler. Disse er meget fleksible, men medfører også lidt administration. Her foregår arbejdet med websiden via en netlæser på en server hos de der leverer tjenesten.

Med Hugo oprettes websiden på din mac/pc, og artiklerne skrives i formatet [Markdown](https://en.wikipedia.org/wiki/Markdown). Teksten oversættes dernæst til HTML. En beskrivelse af formatet findes [her](https://www.markdownguide.org/cheat-sheet/).

Dernæst skal indholdet lægges på en server som er tilgængelig på internettet. [Cloudflare](https://www.cloudflare.com) tilbyder en sådan tjeneste. Cloudflare er en vigtig del af interenttets infrastruktur, hvor de sørger for at indhold sendes frem så hurtig som mulig, beskytter websider som er under angreb med mere.

Det eksempel jeg viser her bruger [Cloudflare Pages](https://pages.cloudflare.com). Websiden sendes dog ikke direkte til Cloudflare, men går via [GitHub](https://github.com) eller [GitLab](https://about.gitlab.com) før det kan vises. Det koster ikke noget at oprette en konto på disse tre tjenester, så websiden kan laves uden at det koster penge.

GitHub og GitLab er virksomheder som du kan laste din kode op til, skrevet i kodeversioneringsværktøjet Git. Koden kan så gøres offentlig så andre kan se den, eller gøres privat, hvis du ikke ønsker andre skal se.
