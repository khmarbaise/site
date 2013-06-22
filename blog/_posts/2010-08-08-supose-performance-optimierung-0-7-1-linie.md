---
layout: post
title: "SupoSE - Performance Optimierung - 0.7.1 Linie"
date: 2010-08-08 18:24:52
tags: SKM,Neuigkeiten,Neue Versionen,Test,SupoSE
categories: SKM,Neuigkeiten,Neue Versionen,Test,SupoSE
post-type: blog
---
<img width='497' height='419' style="float: left; border: 0px; padding-left: 5px; padding-right: 5px;" src="/uploads/supose-multithread-memory-day.png" alt="" />Die <a href="/index.php?/archives/292-Grosser-Test-mit-SupoSE-die-II..html">Optimierung die ich im Ersten Schritt in SupoSE vorgenommen hatte</a> wahren ja schon recht erfolgreich. Von 5 Tagen auf unter 24 Stunden ist ja schon was und gleichzeitig noch den Speicherbedarf reduziert. Aber das war mir noch nicht genug. Also habe ich nochmal nachgedacht was man da denn noch machen kann. Da das Scannen des Repositories ja anhand der Revisionnummern vorgenommen wird war der Schritt in Richtung von BlÃ¶cken a 10.000 Revisions nicht so groÃŸ aber da ist mir die Idee gekommen, da die BlÃ¶cke ja faktisch vollstÃ¤ndig unabhÃ¤ngig voneinander sind, wÃ¤re es ja eigentlich kein Problem auch solche BlÃ¶cke parallel zu bearbeiten. Tja da war die Idee mit multi threading nicht sehr weit. Gesagt getan. Eine erste einfache Implementierung war nicht so aufwendig. Aber das Ergebnis war schlicht und ergreifend entÃ¤uschend. Etwas unter 24 Stunden. Nachdem ich das Ganze dann nochmal genau unter die Lupe genommen hatte, habe ich den ÃœbeltÃ¤ter gefunden. Ich hatte vergessen eine Klasse fÃ¼r jeden Thread neu zu instanzieren. Damit hatte ich mir indirekt eine Synchronisation eingebaut. Nachdem dass angepasst war, war das Ergebnis sehr befriedigend. Anstatt 24 Stunden was das Ganze jetz in ca. 9 Stunden. Das heiÃŸt eine Reduzierung um ca. 2/3 (Na ja nicht so genau nach rechnen ;-)).
Wichtig dabei ist, dass der Rechner (Intel Core i7 mit 12 GB RAM) dabei recht gut Ausgelastet war (siehe Bild). Mit top (Unix Rechner) war auch recht gut zu beobachten, dass die Last auf verschiedene Kerne verteilt wurde. Nachteilig ist selbstverstÃ¤nglich, dass hier wÃ¤hrend des Laufes mehr speicher benÃ¶tigt wird.
<img width='497' height='275' style="float: right; border: 0px; padding-left: 5px; padding-right: 5px;" src="/uploads/supose-multithread-load-day.png" alt="" />

