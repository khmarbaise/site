---
layout: post
title: "Hibernate Annotations: Eigene Sequenzen pro Klasse bei Vererbung"
date: 2008-07-11 20:35:15
tags: Java,Unit Tests,Test
categories: Java,Unit Tests,Test
post-type: blog
---
Bei der Arbeit mit <a href="http://www.hibernate.org"  title="Hibernate">Hibernate</a> tritt hÃ¤ufiger das Problem auf, dass man bei vererbten Klassen pro Tabelle eine eigene Sequence (z.B. in Oracle) verwenden mÃ¶chte bzw. muÃŸ.
Man kann selbstverstÃ¤ndlich die Id in jede Klasse packen und dort dann die entsprechenden Annotierungen anbringen. Das ist aber schlicht und ergreifend lÃ¤sstig und wiederspricht dem OO Prinzip. Wenn man nun konsequent mit Vererbung arbeitet, ergibt es sich, dass meist eine Basis-Klasse entsteht und dort das Id Attribut enthalten ist.