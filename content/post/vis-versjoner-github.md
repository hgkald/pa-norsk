---
title: "Å lære fra feil: Hvordan å vise postversjoner med Github"
date: 2021-03-14T20:09:52+01:00
draft: false
firstversion:
  time: ~90min
  githash: dad9c83f86720cc23d870cab6bfc4080421d8973
tags:
- meta
- Github
kategorier:
- Teknologi
---

Kanskje denne innlegg er litt "meta", men uansett vil jeg beskrive hvordan å se på redigeringer for innleggene her på bloggen.

Det er veldig hjelpsom for å se på skrivefeil, og kanskje dette kan hjelpe dere som vil lage sin egen språkblogg. For eksempel liker jeg å skrive den første versjonen uten eller med veldig få hjelpemidler. Så korrigerer jeg den etterpå, og dermed kan jeg se hvordan å bli bedre.

<!--more-->
## Litt bakgrunn
Først vil jeg beskrive litt hvordan siden fungerer. Hele siden, inkludert innleggene, er lagret på en side som heter *GitHub*. GitHub driver med hovedsakelig for å lagre og dele dataprogrammkode. Kodene er lagret på en format som heter *git*.

En sterk fordel av git er at det er veldig tydelig og enkel å se endringene mellom forskjellige versjoner. Det er en fordel for å vise kode, men også for skriftlige tekst.

## Så hvordan brukes det?
Jeg vil beskrive hvordan å klare det for hver innlegg her. For eksempel kan vi se på innlegget som heter [*Barn og sosiale media*](/post/barn-og-sosiale-medier/).

På slutt av innlegget er en lenk for å vise [*"alle versjoner"*](https://github.com/hgonzal/pa-norsk/commits/master/content/post/barn-og-sosiale-medier.md) (denne innlegg har [en lenke](https://github.com/hgonzal/pa-norsk/commits/master/content/post/vis-versjoner-github.md) også). Når du trykke på det, ser du en liste av versjonene, eller *commits* som git kaller dem:

![Liste av versjoner](/img/barn-innlegg-versjoner.png)

Du kan se at jeg har endret denne siden ganske ofte. Ikke alle er tekstendringer, og mange er endringer til siden selv. For eksempel viser det når jeg endrer designen av bloggen.

Versjonene som er relevant er de som starter med teksten *"Edit post"* (jeg skriver ikke denne notater på norsk :)). For eksempel: en interessant versjon er den som heter *"Edit post: Barn og sosiale medier (edited with native speaker)"*. Det finnes nær enden av listen:

![Se på en spesifikk versjon](/img/barn-innlegg-versjon-highlight.png)

Når du trykke på det, vil du se endringene som jeg har gjort for versjonen:

![Rå tekst](/img/barn-innlegg-raw-endringer.png)

Dette er interessant nok, men det er vanskelig å lese. Heldigvis har allerede GitHub en løsning. Du kan trykke på knappen på det høyre hjørnet av rammen med teksten. Det ser ut som et ark:

![Knappen](/img/barn-innlegg-raw-markdownbox.png)

Voila! Nå kan du se med detaljer hvilke ord og uttrykk ble endret:

![Tekst på rich diff](/img/barn-innlegg-versjon-richdiff.png)

Denne versjon var gjort med samboeren min som korrigert mange ord- og uttrykksfeil. Du kan gjøre denne med alle innleggene på nettsiden.

Jeg vil lage en enklere måte å vise versjoner på, men det er komplisert å implementere. Foreløpig håper jeg at dette er i det minste litt interessant for dere!
