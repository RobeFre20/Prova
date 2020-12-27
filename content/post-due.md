---
title: "Hugo, come creare siti statici"
description: "come creare un sito statico usando un framework di Go"
date: 2020-12-25T12:17:51+01:00
author: "RobertoFretel"
draft: false
type: "post"
image: "images/hugo.svg"
---

Oggi vi farò vedere come creare siti statici utlizzando Hugo, ovvero un framework per generare siti statici in puro html. Si basa sul linguaggio Go ed è molto semplice da utilizzare. Supporta i template ed è possibile scrivere i post in markdown.

Per prima cosa recatevi sul Github ufficiale di Hugo ([clicca qui](https://github.com/gohugoio/hugo/releases)) e, in base al vostro sistema operativo, scaricate l'ultima versione del framework.

Una volta scaricato Hugo, preparate una cartella nel vostro computer dove creare il sito, ed estraete il file appena scaricato dentro ad essa.

###### Bene ora siamo pronti per iniziare!

Ora aprite il terminale all'interno della vostra cartella, scrivendo sulla barra della directory *cmd* e cliccando invio

{{< video >}}https://res.cloudinary.com/robertofre20/video/upload/v1609099387/sito/2020-12-27_21-01-10_i5ek0w.mp4{{< /video >}}

Per creare il sito quindi scriviamo {{< font >}}"hugo new site NOME-DEL-SITO"{{< /font >}} (al posto di NOME-DEL-SITO mettete il nome che volete dare al vostro sito). **D'ora in poi tutte le operazioni saranno solo all'interno della cartella appena creata.**

{{< figure src="https://res.cloudinary.com/robertofre20/image/upload/v1609070433/sito/Cattura2_gf5tnb.png" >}}

Come secondo passo dovrete cercare un tema da caricare nel vostro sito, per farlo cliccate [qui](https://themes.gohugo.io/) e cercate il tema che più vi piace. Una volta trovato il tema cliccate *download*, e nella pagina di Github appena caricata cliccate il pulsante verde *code* e poi *Download ZIP*.

Dopodiché sempre sulla cartella del vostro sito recatevi nella directory *themes* e create una cartella rinominandola *tema*. All'interno di essa estraete il tema appena scaricato.

Come ultimo passaggio aprite il file *config.toml* nella cartella iniziale e aggiungete questa stringa: *theme: "tema"* nell'ultima riga.

{{< figure src="https://res.cloudinary.com/robertofre20/image/upload/v1609083095/sito/Cattura_opja05.png" >}}

N.B.: nel caso la cartella *tema* contenga una cartella chiamata *resources* questa dovrà essere copiata nella directory del sito, sostituendo quella vuota.

###### Abbiamo finito!

Per avviare il sito riaprite il terminale e scrivete il comando {{< font >}}"hugo --config=config.toml"{{< /font >}}

Ovviamente un sito vuoto è inutile.. Per aggiungere dei post o create un nuovo file nella cartella *content* ( solo file markdown | .md ), oppure scrivete nel terminale "*hugo new NOME-DEL-POST.md*"