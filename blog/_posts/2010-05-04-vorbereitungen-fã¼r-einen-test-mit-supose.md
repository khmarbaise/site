---
layout: post
title: "Vorbereitungen fÃ¼r einen Test mit SupoSE"
date: 2010-05-04 21:41:00
tags: SKM,Subversion,Test,SupoSE
categories: SKM,Subversion,Test,SupoSE
post-type: blog
---
Im Rahmen der Test Vorbereitungen fÃ¼r <a href="http://www.supose.org">SupoSE</a> wollte ich mir eine groÃŸes Repository besorgen, damit ich mal das Verhalten mit einem "richtigen" repository testen kann und auch mal ein paar Anhaltspunkte fÃ¼r Zeiten bzgl. eines entsprechenden Repositories bekomme. <br/>
<br/>
Danke der netten Mithilfe der <a href="http://www.apache.org">Apache Software Foundation</a>, gibt es die einfache MÃ¶glichkeit einen <a href="http://svn-master.apache.org/dump/">VollstÃ¤ndigen Dump des Repositories</a> zu erhalten, da ich nicht mit einem svnsync arbeiten wollte, da das zu <a href="https://issues.apache.org/jira/browse/INFRA-2606">groÃŸe kontinuierliche Last erzeugt hÃ¤tte</a>.<br/>
<br/>
Also habe ich den Dump File auf einen Server gelegt und angefangen das Repository per svnadmin load repository <dumpfile zu laden.<br/>
<br/>
Server (Infos: Core i7 CPU;12 <a href="http://de.wikipedia.org/wiki/Gibibyte#Pr.C3.A4fixe_f.C3.BCr_gro.C3.9Fe_Anzahlen_von_Bytes">GiB</a> RAM; 1.3 <a href="http://de.wikipedia.org/wiki/Gibibyte#Pr.C3.A4fixe_f.C3.BCr_gro.C3.9Fe_Anzahlen_von_Bytes">TiB</a> Festplatte)<br/>
<br/>
Download des Dump-Files (930.176 Revs). 10 <a href="http://de.wikipedia.org/wiki/Gibibyte#Pr.C3.A4fixe_f.C3.BCr_gro.C3.9Fe_Anzahlen_von_Bytes">Gib</a> File (http://svn-master.apache.org/dump/)
<br/>
<pre>Icon  Name                               Last modified      Size  Description[DIR] Parent Directory                                        -   
[   ] svn-asf-public-r0:930176.7z        02-Apr-2010 17:02  9.7G  
[   ] svn-asf-public-r0:930176.7z.md5    02-Apr-2010 17:06   79   
[   ] svn-asf-public-r0:930176.7z.sha1   02-Apr-2010 17:09   88   
[   ] svn-asf-public-r0:930176.7z.sha256 02-Apr-2010 17:08  114   
</pre>
</br>
svn-asf-public-r0:930176.7z (10.430.991.745 Bytes) ausgepackt 31.492.319.472 Bytes

Test auf dem  Core I7 ausgefÃ¼hrt:
</br>
svnadmin load
</br>
<ul>
  <li>Started
    <ul><li>Apr 12 21:26 repos/db/revs/0/1</li></ul>
  </li>
  <li>Stopped:
    <ul><li>Apr 25 14:05 repos/db/current</li></ul>
  </li>
  <li>BenÃ¶tigte Zeit:
    <ul><li>12 Tage 16 Stunden 39 Minuten</li></ul>
  </li>
  <li>Repository size nach load
    <ul><li>27.102.128.173 Bytes</li></ul>
  </li>
</ul>

Das gleiche habe ich dann nochmal auf einem anderen Rechner gemacht, um hier einen Vergleich zu haben.
Test auf dem  Intel(R) Core(TM)2 Duo CPU     E8400  @ 3.00GHz (4 GiB RAM)
</br>
svnadmin load
</br>
<ul>
  <li>Started
    <ul><li>Apr 20 23:11 repos/db/revs/0/1</li></ul>
  </li>
  <li>Stopped:
    <ul><li>2. Mai 00:25 repos/db/current</li></ul>
  </li>
  <li>BenÃ¶tigte Zeit:
    <ul><li>11 Tage 1 Stunde und 14 Minuten</li></ul>
  </li>
  <li>Repository size nach load
    <ul><li>27.102.279.725 Bytes</li></ul>
  </li>
</ul>