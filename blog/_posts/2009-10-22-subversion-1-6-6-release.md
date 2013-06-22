---
layout: post
title: "Subversion 1.6.6 Release"
date: 2009-10-22 08:08:06
tags: SKM,Neuigkeiten,Neue Versionen,Subversion
categories: SKM,Neuigkeiten,Neue Versionen,Subversion
post-type: blog
---
Die neue Release von Subversion 1.6.6 ist nun da. Die <a href=" http://subversion.tigris.org/svn_1.6_releasenotes.html">Release Notes</a> geben Auskunft Ã¼ber die grundlegenden Neuerungen in der Release 1.6 wÃ¤hrend der <a href="http://svn.collab.net/repos/svn/tags/1.6.6/CHANGES">ChangeLog</a> die Ã„nderung in der Release 1.6.6 beschreiben. Es wurden wieder einige Bugs behoben.

<ul>
  <li>Ã„nderungen fÃ¼r den Benutzer sichtbar:
  <ul>
  <li>Fixed Absturz wÃ¤hrend 'svn update' (r39673)</li>
  <li>Beachte Apache's ServerSignature Anweisung (r40008, -21, -31)</li>
  <li>Eine Datei mit gemischten Zeilenenden wird nicht hinzugefÃ¼gt (issue #2713)</li>
  <li>UnterstÃ¼tzung fÃ¼r Neon 0.29.</li>
  <li>Fixed Absturz bei 'svn rm --force' (r37953)</li>
  <li>Behandlung eines Tree-Conflicts mit Ersetzungen(issue #3486)</li>
  <li>Erlauben von non-threadsafe sqlite wenn APR keine Threads hat (r39301)</li>
  <li>Ausgabe einer Zeilenumbruch vor dem Plaintext SSL cert / Passwort prompt  (r38982, r39302)</li>
  <li>ErhÃ¶hung der Merge Performance mit implizitem Subtree Mergeinfo (issue #3443)</li>
  <li>Fixed "libsvn_ra_svn/marshal.c assertion Absturz (opt || cstr)" (issue #3485)</li>
  <li>Externals fÃ¼r binÃ¤r Dateien (issue #3368)</li>
  <li>MIME type Erkennung case-insensitively (issue #3479)</li>
  <li>Eine nicht vorhandene Revision wird nicht als HEAD interpretiert bei 'svn export' (issue #3400)</li>
  <li>RÃ¼ckgÃ¤ngig r36720's default MIME type wieder "text/plain" (issue #3508)</li>
  <li>Verbesserung der "tree conflict already exists" Fehlermeldung  (r38872)</li>
  <li>Fixed Problem bei dem committen von Verzeichniss Ersetzungen (issue #3281)</li>
  <li>Fixed mod_dav_svn Eltern Verzeichnis Links zur Erhalutng der Peg-Revision(issue #3425)</li>
</ul>
</li>

<li>Ã„nderungen fÃ¼r Entwickler:
  <ul>
  <li>Fixed zwei Fehlgeschlagene Tests in den Ruby Bindings(r38886)</li>
  <li>Keine Notwendigkeit von GNU grep fÃ¼r den Build (issue #3453)</li>
  <li>Verwendung von '$SED' anstatt  'sed' in den Build Skripten (issue #3458)</li>
  <li>HinzugefÃ¼gt svn.client.{log5,merge_peg3} zu den Python Bindings (r39635, -6, -7)</li>
  <li>Erweiterung des tests.log um die Laufzeit eines Test (r39887)</li>
  </ul>
</li>
</ul>

 