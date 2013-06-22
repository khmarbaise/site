---
layout: post
title: "Subversion 1.5 - Beta 1"
date: 2008-03-14 00:06:13
tags: SKM,Neuigkeiten,Neue Versionen,Subversion
categories: SKM,Neuigkeiten,Neue Versionen,Subversion
post-type: blog
---
Nun wird es langsam Ernst mit Subversion 1.5....<a href="http://subversion.tigris.org/servlets/ReadMsg?list=dev&msgNo=136032"  title="Beta 1">die erste Beta Version</a> ist erschienen und sollte gut getestet werden....<br/>
Was bietet Subversion 1.5. denn nun so neues?
<ul>
<li>Tja zuerst einmal, das viel gewÃ¼nschte (Enterprise) Feature Merge-Tracking...
<p>Es ist also nicht mehr nÃ¶tig, die gemergten Versionen in der Log-Message zu notieren...das erledigt nun Subversion selbst.</p>
<p>Es ist auch mÃ¶glich Changes nicht zu mergen (<a href="http://svnbook.red-bean.com/nightly/en/svn-book.html#svn.branchmerge.advanced.blockchanges"  title="Block Changes">Blocking changes</a>)</p>
</li>
<li><p>Dann gibt es noch so Dinge wie <a href="http://svnbook.red-bean.com/nightly/en/svn-book.html#svn.advanced.changelists"  title="ChangeLists">ChangeLists</a>, die dazu dienen, zusammen gehÃ¶rige Dateien etc. als eine Einheit betrachten zu kÃ¶nnen. Damit wird die Arbeit in der Working Copy(WC) vereinfacht hier an z.B. zwei Changes gleichzeitig in einer WC zu arbeiten. Bei einem Commit kann dann die ChangeList bennannt werden. Damit werden dann nur die Dateien commited die zur jeweiligen ChangeList gehÃ¶ren.</p></li>
<li><p>Ach ja da war ja noch das Thema mit der KonfliktbewÃ¤ltigung Ã¤hm..sorry Konflikt Behandlung. Das kann dann auftauchen, wenn svn update ausgelÃ¶st wurde und andere Kollegen hier Ã„nderungen durchgefÃ¼hrt haben (Was ja nicht unÃ¼blich ist, andere arbeiten ja auch ;-)).</p>
<p>Dann ist es mÃ¶glich diese <a href="http://svnbook.red-bean.com/nightly/en/svn-book.html#svn.tour.cycle.resolve"  title="Interactive conflict resolution">Interaktiv in die WC</a> einzuarbeiten und nicht wie bisher alles oder nichts. Subsumiert wird das Ganze dann unter <b>Interactive conflict resolution</b></p>
<p><a href="http://svnbook.red-bean.com/nightly/en/svn-book.html#svn.advanced.sparsedirs"  title="Sparse-Checkouts">Sparse-Checkouts</a>, Write-Through Proxy und wie ich finde noch eine recht interessante Ã„nderung, nÃ¤mlich dass svn:externals nun auch mit relativen Angaben arbeiten kÃ¶nnen.....</p>
<p>Und ganz viele Bug-Fixing</p>
<li>Den derzeitigen Stand des ChangeLog's....kann man <a href="http://svn.collab.net/repos/svn/trunk/CHANGES"  title="ChangeLog Beta1">hier</a> finden </li>
</ul>