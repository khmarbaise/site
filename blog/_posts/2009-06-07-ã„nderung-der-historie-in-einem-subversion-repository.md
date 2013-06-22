---
layout: post
title: "Ã„nderung der Historie in einem Subversion Repository"
date: 2009-06-07 15:27:33
tags: SKM,Neuigkeiten,Subversion
categories: SKM,Neuigkeiten,Subversion
post-type: blog
---
Tja ich hatte das Problem, dass ich aus versehen in einer Datei etwas geschrieben hatte, was da nicht reingehÃ¶rt (Klassiker ist hier ein Paasword fÃ¼r Datenbanken etc.) und zu allem UnglÃ¼ck habe ich das dann auch noch in ein Subversion Repository eingecheckt. Tja wie bekomme ich das jetzt wieder da raus...<br/>
Es gibt zum glÃ¼ck ein <a href="http://svn.borg.ch/svndumptool/">nettes Tools</a> mit dem man ein solches Problem lÃ¶sen kann. Damit ist es mÃ¶glich aus einem Subversion Dump File den Inhalt einer Datei durch einen anderen zu ersetzen.
<pre>svndumptool.py edit -r Revision -f PfadImRepository/Datei --replace=dateineu original.dump korrigiert.dump</pre>.
Danach muss man einfach nur den <b>korrigiert.dump</b> wieder in ein leeres Repository per <pre>svnadmin load neu &lt;korrigiert.dump</pre> einspielen. 
