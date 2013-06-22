---
layout: post
title: "Subversion 1.5.5 - Erschienen"
date: 2008-12-22 22:34:00
tags: SKM,Neuigkeiten,Neue Versionen,Subversion
categories: SKM,Neuigkeiten,Neue Versionen,Subversion
post-type: blog
---
Das <a href="http://subversion.tigris.org/">Subversion Team</a> hat <a href="http://subversion.tigris.org/servlets/NewsItemView?newsItemID=2223">bekannt gegeben</a>, dass nun die <a href="http://svn.collab.net/repos/svn/tags/1.5.5/CHANGES">Release 1.5.5</a> von Subversion zur VerfÃ¼gung steht. 

<ul>
  <li>Ã„nderungen, die fÃ¼r den Anwender sichtbar sind:
  <ul>

   <li>Der commit wird nun ermÃ¶glicht wenn Properties geÃ¤ndert wurden, aber verÃ¤nderte Unterverzeichnisse existieren (r34487, -92, -94)</li>
   <li>Cyrus Authentifizierung bevorzugt nun immer EXTERNAL vor ANONYMOUS (r33866)</li>
   <li>Erzeuge keine Mergeinfo's fÃ¼r verschieben/kopieren innerhalb einer Arbeitskopie  (r34184, -585)</li>
   <li>Kein automatisches Upgrade von alten Berkeley DB Dateisystem auf 1.5 oder 1.4 Format (r34653, -6)</li>
   <li>RÃ¼ckgabe von Mergeinfos des vorherigen Zustandes wÃ¤hrend eines reverse Merges(r30257, r33024, -6)</li>
   <li>Entfernung von Merginfo die durch merge gelÃ¶scht wurde (ssue #3323)</li>
   <li>ErmÃ¶gliche den Proxy Slave's das Durchkommen der txn GET und PROPFIND Requests (issue #3275)</li>
   <li>Merge kann nun Zielen mit inkonsitenten ZeilenumbrÃ¼chen verwenden (issue #3262)</li>
   <li>Unterbindung von leeren ChangeListen (issue #3344)</li>
   <li>Entfernung von falschen positiven ra_neon Merginfo Fehlern (r34822)</li>
   <li>ErhÃ¶hung der Performance von 'svn merge --reintegrate' (r34091, -4, and others)</li>
   <li>Korrektur: Fremde Merges erhalten UUID des fremden Repositories (r34050, -1, -3)</li>
   <li>Korrektur: Verwendung von korrekt kodierten diff-Headers in der Konflikt AuflÃ¶sung(r34171)</li>
   <li>Korrektur: Segmentation Fault in 'svn cp --parents' (r31311, -4)</li>
   <li>Korrektur: Mergeinfos fÃ¼r leere Revision Bereichsangabe  (issue #3312)</li>
   <li>Korrektur: Segmentation Fault in BDB Backend fÃ¼r Node-Origins Cache (r34506)</li>
   <li>Korrektur: Fehlerhafter Merge wenn die Zielhistorie wiederherstellungen erhÃ¤lt(r34385, -93)</li>
   <li>Korrektor: UngÃ¼ltige Mergeinformationen die bei einem Mergevorgang von einem Unterbaum erzeugt wurden (r34560, -2)</li>
   </ul>

  <li>Ã„nderungen fÃ¼r Entwickler:
   <ul>
     <li>Korrektur: svn_repos_get_logs() Fehler bei verschiedenen Revision Parametern.(r33873, -4)</li>
  </ul>
</ul>
