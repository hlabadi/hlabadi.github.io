---
title: "Strava embed"
description: "meta"
publishDate: "23 Aug 2025"
---

Szóval, a Strava embednek működnie kellene. HTML-t ad, de ide viszont Markdown kell.

<div class="strava-embed-placeholder" data-embed-type="activity" data-embed-id="15515614553" data-style="standard" data-from-embed="false"></div><script src="https://strava-embeds.com/embed.js"></script>

Viszont működik. Miért? Mert a Markdown hülyén mondva a HTML fölé épül:

> For any markup that is not covered by Markdown’s syntax, you simply use HTML itself. There’s no need to preface it or delimit it to indicate that you’re switching from Markdown to HTML; you just use the tags.

Ez gyors volt. Bárcsak minden ilyen egyszerűen menne.

Ami érdekes, hogy úgy tűnik a thumbnaileket nem támogatja az embed, pedig a Fitness+ elég jókat generál.

<div class="strava-embed-placeholder" data-embed-type="activity" data-embed-id="15528131750" data-style="standard" data-from-embed="false"></div><script src="https://strava-embeds.com/embed.js"></script>

Na mindegy, close enough.

Legközelebb a kígyókról lesz szó.