---
layout: post
title: "Ruby on Rails mit Apache / Mongrels Cluster "
date: 2009-04-03 12:49:00
tags: Neuigkeiten,Redmine
categories: Neuigkeiten,Redmine
post-type: blog
---
<a class='serendipity_image_link' href='/uploads/load.png'><img width='110' height='59' style="float: left; border: 0px; padding-left: 5px; padding-right: 5px;" src="/uploads/load.serendipityThumb.png" alt="" /></a>Tja, nachdem ich nun beobachtet habe, wie es zu hÃ¤ufigeren Ausssetzern kommen, habe ich mich nun entschieden die Kombination Apache / Mongrels Cluster durch etwas anderes zu ersetzten. Es ist nÃ¤mlich hÃ¤ufiger zu beobachten (siehe bild), dass sich der Load des Servers in schlagartig erhÃ¶ht. Ich habe die Anzahl der Mongrels Knoten schon von zwei auf fÃ¼nf erhÃ¶ht, da ich vermutete, dass es notwendig ist  mehr Knoten zur VerfÃ¼gung zu stellen.<br/>
<br/>
<div class="serendipity_imageComment_left" style="width: 110px"><div class="serendipity_imageComment_img"><a class='serendipity_image_link' href='/uploads/load20090218.png'><img width='110' height='59'  src="/uploads/load20090218.serendipityThumb.png" alt="" /></a></div><div class="serendipity_imageComment_txt">Load am 18.02.2009</div></div>Tja wie es aussieht hat die ErhÃ¶hung der Knoten nicht wirklich geholfen. Das hat jetzt einen Load Wert von max. 15.8 auf der Maschine erzeugt.
Jetzt ist es tatsÃ¤chlich Zeit etwas andere zu installieren.
<br/>
<br/>
<br/><br/><br/><br/>
<a class='serendipity_image_link' href='/uploads/redmine-load-20090403.png'><img width='110' height='59' style="float: left; border: 0px; padding-left: 5px; padding-right: 5px;" src="/uploads/redmine-load-20090403.serendipityThumb.png" alt="" /></a><strong>[Update]</strong>Also die Geschichte wird nicht besser....