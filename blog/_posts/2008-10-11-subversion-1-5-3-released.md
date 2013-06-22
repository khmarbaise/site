---
layout: post
title: "Subversion 1.5.3 - Released"
date: 2008-10-11 11:08:00
tags: SKM,Neue Versionen,Subversion
categories: SKM,Neue Versionen,Subversion
post-type: blog
---
Nun ist es so weit, es gibt einen neue Release von <a href="http://subversion.tigris.org/servlets/NewsItemView?newsItemID=2164"  title="Subversion 1.5.3">Subversion 1.5.3</a>.

Die <a href="http://subversion.tigris.org/svn_1.5_releasenotes.html"  title="Release Notes">Release Notes</a> beschreiben die Ã„nderungen insgesamt und der <a href="http://svn.collab.net/repos/svn/tags/1.5.3/CHANGES"  title="Change Log">Change Log</a> genau die Ã„nderungen pro Release.

<ul>
<li>User-visible changes:</li>
<ul>
<li>Fortsetzung switch nach der lÃ¶schung von lokal modifizierten Verzeichnissen(issue #2505)</li>
<li>Update der bash_completion fÃ¼r die KompatibilitÃ¤t mit 1.5 (r32900, -11, -12)</li>
<li>Verbesserung von 'svn merge' AusfÃ¼hrungszeit um 30% auf Windows (r33447)</li>
<li>Wiederverwendung der Netzwerk Session wÃ¤hrend 'svn merge', Verbesserung der Performancer(r33476)</li>
<li>Verbesserung der tempÃ¤r Datei Erzeugungszeit auf Windows(r33464)</li>
<li>GroÃŸe Verbesserung der merge Performance (r29969, r32463, r33013, -016, -022, -112)</li>
<li>Verbesserung der Datei I/O Performance auf Windows (r33178, -85)</li>
<li>Korrigiert: Merging von Dateinamen mit Spaces im Namen  (r33109, -121, -369)</li>
<li>Korrigiert: ungÃ¼ltige reltive externals Erweiterung incorrect relative (r33109, -121, -369)</li>
<li>Korrigiert: 'svn mv' HÃ¤nger und Memory Leack(r33201, -12)</li>
<li>Korrigiert: Nachverfolgung in 'svn log -g' (issue #3285)</li>
<li>Korrigiert: Aktuellen frÃ¼hen 'bailout' von 'svn log -g' (r32977)</li>
</ul>

<li>Developer-visible changes:
<ul>
<li>Tests kÃ¶nnen auch als nicht Admin laufen gelassen werden (Windows Vista) (r31203)</li>
<li>ErmÃ¶glichung der Compilierung ausserhalb Allow out-of-tree build of bindings on BSD (r32409)</li>
<li>Ãœbersetzung der Nachrichten  in svn_fs_util.h (r32771)</li>
<li>Korrigiert: Bindings fÃ¼r Perl 5.10 (r31546)</li>
<li>Korrigiert: Ãœbersetzung der Bindings der C API Test s mit VS2008 (r32012)</li>
<li>Korrigiert: svn_ra_replay API Ã¼ber ra_serf (r33173)</li>
</ul>
</ul>

