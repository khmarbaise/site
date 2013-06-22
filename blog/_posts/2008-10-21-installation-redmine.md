---
layout: post
title: "Installation Redmine"
date: 2008-10-21 20:56:10
tags: Neuigkeiten,Redmine
categories: Neuigkeiten,Redmine
post-type: blog
---
Ich habe die Schritte zur Installation von <a href="http://www.redmine.org">Redmine</a> einmal aufgefÃ¼hrt, damit man sieht wie einfach es ist Redmine zu installieren. Ich habe mich dafÃ¼r entschieden Redmine auf einer MySQL zu betreiben.
<ul>
<li>Installation MySQL 5.0</li>
<li>Installation Ruby (1.8.6)</li>
<li>Donwload <a href="http://rubyforge.org/frs/?group_id=126&release_id=26453">gems (1.3.0)</a>; Danach ein einfaches <pre>ruby ./setup.rb</pre></li>
<li>gem install rails -v 2.1.1 (Hier muss -v 2.0.1 angegeben werden, wenn mit der 0.7.3 Releasae gearbeitet werden soll)</li>
<li><a href="http://www.redmine.org/wiki/redmine/CheckingoutRedmine">Auschecken einer Entwicklungsversion</a> per <pre>svn checkout http://redmine.rubyforge.org/svn/trunk</pre></li>
<li>Installation der DB laut <a href="http://www.redmine.org/wiki/redmine/RedmineInstall">Anleitung von Redmine</a><pre>create database redmine character set utf8;</pre></li>
<li>Wechsel in das vorher ausgecheckte Verzeichnis; Initialisierung der Datenbank.<pre>rake db:migrate RAILS_ENV="production"</pre></li>
<li>Default Konfiguration einspielen<pre>rake redmine:load_default_data RAILS_ENV="production"</pre></li>
<li>Start via ruby script/server -p 80 production</li>
</ul>
Das wars....