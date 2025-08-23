---
title: "JavaScript delete"
description: "dev"
publishDate: "24 Aug 2025"
---

Kb fél éve az irodában TypeScriptben fejlesztek. Előtte soha nem nyúltam a JS/TS pároshoz. Nem az én világom volt, meghát ott volt a dotnetes felsőbbrendűség is, hogy nehogy már olyan nyelven írjak, ahol 100 + '100' = 100100. Aztán valahogy megtetszett. Mellé jött egy React Native keretrendszer (vagy minek hívják őket odaát), minden funkcionális nyalánksággal. Nem mondom, elejében nagyon kapkodtam a fejem, de aztán szerintem elég produktívvá váltam.

Na de, mivel elég rohamtempóban történt a betanulás, egy csomó minden kimaradt. Épp olvastam a vonaton hiánypótlásból az [Essential TypeScript 5, Third Edition](https://www.manning.com/books/essential-typescript-5-third-edition) című könyvet és van két JavaScript fejezet benne. Itt volt arról szó, hogy JS-ben ugye az objektum/osztály dolog elég képlékeny dolog, alapból alakjuk(?) van csak. És ha nem matchel teljesen az elvártra, hát az sem nagy gáz.

Na de.

Olyat is tudunk csinálni, hogy van egy példányunk. Nem is tudom, objektum, dotnetben példány, de itt egy névtelen osztály példánya. Mindegy. Szóval vagy egy _cirmi_ példányunk.

```
const cirmi = {
    labak: 4,
    minta: 'cirmos',
    dorombolasHangero: 1
}

```

Ha kiloggoljuk, akkor az lesz belőle, hogy:

```
console.log('cirmi OG', JSON.stringify(cirmi));
```

> cirmi OG {"labak":4,"minta":"cirmos","dorombolasHangero":1}

és most jön a mágia. Úgy döntünk, hogy áh, mégis, milyen hülyeség, nem kell nekünk az a dorombolás hangerő. Mit csinálunk dotnetben? Hát, ha feltételezzük, hogy egy névtelen példány, akkor kézzel átmásolgatjuk a propertyket, kihagyva azt, ami nem kell. De itt?

```
delete cirmi.dorombolasHangero;
console.log('cirmi bionic', JSON.stringify(cirmi));
```

Ennyi. Mi lesz ebből, ha kiloggoljuk?

> cirmi bionic {"labak":4,"minta":"cirmos"}

Borzasztó érdekes. Be kell vallanom, egyre inkább tetszik ez az egész. Alig várom, hogy hétfőn ismét ebben tudjak tákolni.