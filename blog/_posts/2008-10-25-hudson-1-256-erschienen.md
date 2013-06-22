---
layout: post
title: "Hudson - 1.256 - Erschienen"
date: 2008-10-25 18:16:23
tags: Neue Versionen,Hudson
categories: Neue Versionen,Hudson
post-type: blog
---
Es ist eine aktualisierte Release der Continous Integration LÃ¶sung <a href="https://hudson.dev.java.net/">Hudson</a> erschienen.
Der <a href="https://hudson.dev.java.net/changelog.html">ChangeLog</a> gibt genaue Auskunft Ã¼ber die bisherigen Ã„nderungen. Die aktuelle Release behebt einige kleinere Probleme:
<ul>
<li>FÃ¤lchlicherweise waren zwei dom4j.jar's enthalten, welche zu Problemen mit WebSphere fÃ¼hrten (Issue 2435)</li>
<li>Korrektur einer NPE im Falle einer fehlerhaften changelog.xml Datei (issue 2428)</li>
<li>Verbesserte Fehler Erkennung bei der Verwendung von Windows Pfadangaben auf einem Unix Slave(report)</li>
<li>Automatisches AbhÃ¤ngigkeits Management von Maven Projekten kann nun deaktiviert werden (Issue 1714)</li>
</ul>
Zu bekommen ist Hudson im <a href="https://hudson.dev.java.net/servlets/ProjectDocumentList?folderID=2761&expandFolder=2761&folderID=0">Download Bereich.</a>