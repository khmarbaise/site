---
layout: post
title: "Subversion 1.5.3 - Released"
date: 2008-10-11 11:08:00
tags: SKM,Neue Versionen,Subversion
categories: SKM,Neue Versionen,Subversion
post-type: blog
---
Nun ist es so weit, es gibt einen neue Release von <a href="http://subversion.tigris.org/servlets/NewsItemView?newsItemID=2164"  title="Subversion 1.5.3">Subversion 1.5.3</a>.

Die <a href="http://subversion.tigris.org/svn_1.5_releasenotes.html"  title="Release Notes">Release Notes</a> beschreiben die Änderungen insgesamt und der <a href="http://svn.collab.net/repos/svn/tags/1.5.3/CHANGES"  title="Change Log">Change Log</a> genau die Änderungen pro Release.

<ul>
<li>User-visible changes:</li>
<ul>
<li>Fortsetzung switch nach der löschung von lokal modifizierten Verzeichnissen(issue #2505)</li>
<li>Update der bash_completion für die Kompatibilität mit 1.5 (r32900, -11, -12)</li>
<li>Verbesserung von 'svn merge' Ausführungszeit um 30% auf Windows (r33447)</li>
<li>Wiederverwendung der Netzwerk Session während 'svn merge', Verbesserung der Performancer(r33476)</li>
<li>Verbesserung der tempär Datei Erzeugungszeit auf Windows(r33464)</li>
<li>Große Verbesserung der merge Performance (r29969, r32463, r33013, -016, -022, -112)</li>
<li>Verbesserung der Datei I/O Performance auf Windows (r33178, -85)</li>
<li>Korrigiert: Merging von Dateinamen mit Spaces im Namen  (r33109, -121, -369)</li>
<li>Korrigiert: ungültige reltive externals Erweiterung incorrect relative (r33109, -121, -369)</li>
<li>Korrigiert: 'svn mv' Hänger und Memory Leack(r33201, -12)</li>
<li>Korrigiert: Nachverfolgung in 'svn log -g' (issue #3285)</li>
<li>Korrigiert: Aktuellen frühen 'bailout' von 'svn log -g' (r32977)</li>
</ul>

<li>Developer-visible changes:
<ul>
<li>Tests können auch als nicht Admin laufen gelassen werden (Windows Vista) (r31203)</li>
<li>Ermöglichung der Compilierung ausserhalb Allow out-of-tree build of bindings on BSD (r32409)</li>
<li>Übersetzung der Nachrichten  in svn_fs_util.h (r32771)</li>
<li>Korrigiert: Bindings für Perl 5.10 (r31546)</li>
<li>Korrigiert: Übersetzung der Bindings der C API Test s mit VS2008 (r32012)</li>
<li>Korrigiert: svn_ra_replay API über ra_serf (r33173)</li>
</ul>
</ul>

