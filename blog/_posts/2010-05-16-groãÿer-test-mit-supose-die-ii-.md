---
layout: post
title: "GroÃŸer Test mit SupoSE die II."
date: 2010-05-16 12:04:41
tags: SKM,Neuigkeiten,SupoSE
categories: SKM,Neuigkeiten,SupoSE
post-type: blog
---
Nach der Beurteilung der Test Ergebnisse insbesondere der Laufzeiten habe ich mir <a href="http://www.supose.org/repositories/revision/supose/479">einige optimierungen fÃ¼r SupoSE Ã¼berlegt</a> und nun in einem Test auf die gleichen Test Daten losgelassen. Wichtig dabei ist zum einen, dass die Geschwindigkeit enorm gesteigert wurde (aber warten wir mal das Ende ab) und dass hier mit den Default Einstellungen fÃ¼r den Speicher gearbeitet wurde (-Xms512m -Xmx1024m). 

<ul>
  <li>
    <ul><li>scan gestartet: 15.05.2010 20:37:54</li></ul>
    <ul><li>Laufzeit bis dato: 16.05.2010 12:00:00</li></ul>
    <ul><li>Bisher ca. 710.000 Revisions gescanned</li>
     </ul>
  </li>
</ul>
Das heiÃŸt nach bisheriger Ãœbersicht dass innerhalb von weniger als 16 Stunden schon Ã¼ber 700.000 Revisions gescanned worden sind.<br/>
<br/>
<strong>Update: 19:32 Uhr. Alle 94 Indizes gemerged (3877 Sekunden)</strong>
<br/>
<strong>Update: 18:27 Uhr. Derzeitiger Stand: 930.176 Revisions gescanned.</strong>
<br/>
<strong>Update: 17:36 Uhr. Derzeitiger Stand: 900.000 Revisions gescanned.</strong>
<br/>
<strong>Update: 16:10 Uhr. Derzeitiger Stand: 830.000 Revisions gescanned.</strong>
<br/>
<strong>Update: 14:30 Uhr. Derzeitiger Stand: 780.000 Revisions gescanned.</strong>
<br/>
<strong>Update: 13:33 Uhr. Derzeitiger Stand: 750.000 Revisions gescanned.</strong>

<br/>
<br/>
<br/>
Zusammenfassung des Ganzen. Zum einen ist nun die vollstÃ¤ndige Zeit zur Indizierung etc. auf unter 24 Stunden gefallen. Nachteil ist derzeit, dass der Plattenplatz Bedarf auf ca. 110 <a href="http://de.wikipedia.org/wiki/Bin%C3%A4rpr%C3%A4fix">GiB</a> zwischenzeitlich gestiegen ist. Die einzelnen Indizes habe ich derzeit noch nicht automatisch gelÃ¶scht. Das heiÃŸt, dass hier nochmal ca. 55 GiB dazu kommen.
