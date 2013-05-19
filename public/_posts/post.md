---
layout: default
title: Vorträge
---

<div id="home">
  <h1>My Lecutres</h1>
  <ul class="posts">
    {% for post in site.posts %}
      {% if post.post-type == 'lecture' %}
        <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
      {% endif %}
    {% endfor %}
  </ul>
</div>


<h2><a href="http://2009.subconf.de/startseite/">Vortr&auml;ge auf der dritten Subversion Konferenz in M&uuml;nchen</a></h2>
<p>Auf der 3. Subversion Konferenz hatte ich das Vergn&uuml;gen insegesamt vier Vortr&auml;ge halten zu d&uuml;fen.</p>

<ol>
	<li>
		<h3><a href="http://2009.subconf.de/vortragsuebersicht/marbaise-3/">Versionierung in Java</a></h3>
		<p>SVNKit ist in vielen Anwendungen wie z.B. Eclipse vertreten und erm&ouml;glicht mit Java den Zugriff auf 
			Subversion Repositories und die Nutzung von Arbeitskopien. Aber wie funktioniert das? 
			Wie kann man das mit SVNKit selbst machen? Der Vortrag soll helfen zum einen die m&ouml;glichen Anwendung von 
			SVNKit zu verstehen aber auch die M&ouml;glichkeit bieten eigene Anwendungen mit Unterst&uuml;tzung von 
			Subversion bzw. SVNKit zu entwickeln. Wie kann z.B. ein Checkin mithilfe von SVNKit durchgef&uuml;hrt 
			werden oder wie kann ein Change Set ausgelesen werden?</p>
		<a href="/files/SubConf2009SubversionJava.pdf" target="_blank">Versionierung in Java (PDF)</a>
	</li>
	<li>
		<h3><a href="http://2009.subconf.de/vortragsuebersicht/marbaise-4/">To be DVCS or not to be</a></h3>
		<p>Es gibt unterschiedliche Versionskontroll Werkzeuge die auf unterschiedlichen Ans&auml;tzen beruhen wie z.B. git, 
			mercurial usw. and z.B. auch Subversion aber was sind die Vor- bzw. Nachteile solcher Werkzeuge?
			Welches sind die Grundlegenden Konzepte von verteilten- bzw. zentralisierten Versionskontroll Werkzeugen?</p>
		<a href="/files/SubConf2009DVCSvsCVCS.pdf" target="_blank">To be DVCS or not to be (PDF)</a>
	</li>
	<li>
		<h3><a href="http://2009.subconf.de/vortragsuebersicht/marbaise-2/">Die Qual der Versionen die 2.</a></h3>
		<p>H&auml;ufig tritt das Problem auf, dass nach bestimmten Dateien oder Inhalten innerhalb von Subversion 
			Repositories gesucht werden muss.  Mithilfe von vorhandenen Frameworks wie z.B. Lucene, Quartz, SVNKit etc. ist 
			es m&ouml;glich eine Suchmaschine zu erstellen, die mehrere Repositories scannt und die Inhalte zur Verf&uuml;gung
			stellt und somit eine Suche innerhalb von mehreren Repositories erm&ouml;glicht. Damit ist es sehr einfach
			m&ouml;glich, Inhalte etc. einfach und schnell zu suchen.</p>
			<p>SupoSE (Subversion Repository Search Engine) bietet genau diese Funktionalit&auml;t.
			Sinn und Zweck ist es, die Suchmaschine und deren Konzept vorzustellen und auch, welche 
			M&ouml;glichkeiten geboten werden und welche nicht. Hier w&auml;ren R&uuml;ckmeldungen der Besucher 
			hilfreich, um zu sehen, welche Erweiterungen ben&ouml;tigt werden und welche nicht. 
		</p>
		<a href="/files/SubConf2009SupoSE.pdf" target="_blank">Subversion Repository Search Engine (SupoSE) (PDF)</a>
	</li>
	<li>
		<h3><a href="http://2009.subconf.de/vortragsuebersicht/marbaise/">Software Collaboration</a></h3>
		<p>Es gibt unterschiedliche Tools, um die Zusammenarbeit im Rahmen einer Softwarentwicklung zu verbessern. 
		Dazu z&auml;hlen sog. Software Collaborations L&ouml;sungen. Hier sind aus dem Bereich OpenSource z.B. Trac, 
		Redmine, FusionForge  (ehemals GForge) zu nennen. Im Rahmen des Vortrags wird Redmine dargestellt, welche Vor- und Nachteile 
		die es hat. Dazu z&auml;hlt beispielsweise die Installation und die Integration mit anderen Werkzeugen z.B.  
		mit der Versionskontrolle (z.B. Subversion) weiterhin wird gezeigt welche Arten der Konfiguration 
		m&ouml;glich ist und wie Redmine in der T&auml;glichen Anwendung zu nutzen ist. 
		</p>
		<a href="/files/SubConf2009Redmine.pdf" target="_blank">Redmine (PDF)</a>
	</li>
</ol>


<h2><a href="http://www.gearconf.de/die-gearconf-09">Vortr&auml;ge auf der Gearconf 2009 in D&uuml;sseldorf</a></h2>

<ol>
<li><h3>Redmine ein Projekt-Management-Tool</h3>
		<p>Unter den verschiedenen Werkzeugen, die die Zusammenarbeit bei der Software-Entwicklung unterst&uuml;tzen, 
		gibt es die Gruppe der <b>Software-Collaboration-Tools</b>; im Bereich OpenSource z.B. Trac und Redmine.
		Im Vortrag werden die Vor- und Nachteile von Redmine demonstriert, wie etwa bei der Installation und Integration 
		mit anderen Tools wie Versionskontroll-Systeme (Subversion). Weiterhin wird die Konfiguration erl&auml;utert 
		und der Einsatz des Tools bei der laufenden Arbeit.</p>
<a href="/files/GearConf2009Redmine.pdf" target="_blank">Redmine - ein Projekt-Management-Tool (PDF)</a>
</li>

<li><h3>Die Qual der Versionen</h3>
		<p>H&auml;ufig tritt das Problem auf, dass nach bestimmten Dateien oder Inhalten innerhalb von Subversion Repositories 
		gesucht werden muss. Mithilfe von vorhandenen Frameworks wie z.B. Lucene, Quartz, SVNKit etc. ist es m&ouml;glich, 
		eine Suchmaschine zu erstellen, die mehrere Repositories scannt und die Inhalte zur Verf&uuml;gung stellt und somit 
		eine Suche innerhalb von mehreren Repositories erm&ouml;glicht. Damit ist es sehr einfach m&ouml;glich, 
		Inhalte etc. einfach und schnell zu suchen. <a href="http://www.supose.org">SupoSE (Subversion Repository Search Engine)</a>
		 bietet genau diese Funktionalit&auml;t. Im Vortrag werden die Suchmaschine und deren Konzept vorgestellt und gezeigt, 
		welche M&ouml;glichkeiten geboten werden und welche nicht.</p>
		<a href="/files/GearConf2009SupoSE.pdf" target="_blank">Subversion Repository Search Eingine (SupoSE) (PDF)</a>
</li>
</ol>

<h2><a href="http://www.linuxtag.org/2009/">Vortr&auml;ge auf dem Linux Tag Berlin 2009</a></h2>

<ol>
	<li><h3><a href="http://www.linuxtag.org/2009/de/program/freies-vortragsprogramm/rednerliste/vortragsdetails.html?talkid=161">Der Weisheit letzter Schluss: Maven 2 in der Java Entwicklung</a></h3>

	<p>Im Bereich der Java Entwicklung hat sich in der Zwischenzeit Maven 2 als neuer Standard gegen&uuml;ber dem 
		bisherigen Ant durchgesetzt. Die Gr&uuml;nde daf&uuml;r liegen klar auf der Hand. Die Erstellung eines Build Prozesses mit 
		Maven gestaltet sich in der Regel einfacher und bietet von Anfang an mehr M&ouml;glichkeiten. Es ist m&ouml;glich, 
		die Erstellung eines JAR-Files mit sehr wenig Maven 2 Konfiguration zu bewerkstelligen. In diesem Zusammenhang 
		wird out-of-the-Box ein Unit Test geboten. Wichtig ist dabei, dass man sich das Basis Konzept von Maven zu eigen macht: 
		Konvention über Konfiguration. Das bedeutet, dass die Java Projekte in einer bestimmten Art und Weise organisiert sein m&uuml;ssen. 
		Das f&auml;ngt bei der Verzeichnisstruktur an, geht &uuml;ber den Unit- und Integrationstest, Paketierung und h&ouml;rt beim 
		Deployment auf. Der Vortrag stellt die grundlegende Vorgehensweise dar, um einen Build auf Maven aufzubauen. 
		Dazu geh&ouml;rt die Kompilierung der Java Quellen. Der n&auml;chste Schritt ist die Integration eines Unit 
		Tests in den Build, wie und wann der abl&auml;uft. Danach folgt die Paketierung und wie man spezifische 
		Anforderungen zur Paketierung erf&uuml;llen kann. Ein weitere Schritt ist die Implementierung eines Integrationstests 
		und zu guter Letzt das Deployment von entsprechenden Artefakten.</p>

	<a href="/files/LinuxTagBerlin2009Maven2.pdf">Der Weisheit letzer Schluss: Maven 2 in der Java Entwicklung (PDF)</a>
	</li>

	<li><h3><a href="http://www.linuxtag.org/2009/de/program/freies-vortragsprogramm/rednerliste/vortragsdetails.html?talkid=128">Redmine, das Projekt Management Werkzeug</a></h3>
	<p>Die Notwendigkeit eines Projektmanagement Werkzeuges ist heute nicht mehr die Frage sondern welches?
	Es gibt verschiedene Werkzeuge, um die &Uuml;bersicht innerhalb eines Projektes zu behalten. 
	Der Vortrag geht auf die Installation von Redmine ein, um eine Einsch&auml;tzung für einen konkreten Einsatz zu bekommen. 
	Das bedeutet, dass auch die Komplexit&auml;t der Installation betrachtet wird und selbstverst&auml;ndlich auch der Zeitaufwand. 
	Der n&auml;chste Schritt ist der Bereich der Administration und Einrichtung von Projekten, die mit Redmine verwaltet 
	werden sollen. Dabei geht es darum, welche M&ouml;glichkeiten der Konfiguration bestehen und welche Grenzen in Redmine 
	existieren. Der Bereich der Nutzung wird detailliert beleuchtet, um genau die M&ouml;glichkeiten zu sehen, die Redmine bietet. 
	Hier wird betrachtet, wie die Interaktion mit Versionskontrollwerkzeugen von statten geht und auch der Workflow von Issues 
	(z.B. Bugs, ToDo's, Patches). Es wird gezeigt, wie mithilfe des integrierten Wiki's entsprechende Dokumentationen 
	f&uml;r Projekte erstellt werden k&ouml;nnen und wie die Verkn&uml;pfung der unterschiedlichen Bereich untereinander durchgef&uuml;hrt 
	wird. Die &Uuml;bersicht über ein Projekt kann sehr einfach durch die Betrachtung der Roadmap geschehen. Die Roadmap kann 
	nat&uml;rlich auch zur Planung eines Projektes eingesetzt werden. Dazu dient auch zus&auml;tzlich die M&ouml;glichkeit Gantt Charts 
	zu erzeugen und die Integration in den Kalender. In Redmine ist auch eine recht einfache aber sehr effektive 
	Aufwandserfassung enthalten, die zur Erstellung von Berichten genutzt werden kann und somit einen weiteren Baustein 
	zum Projektmanagement beitr&auml;gt. Die weiteren Bereiche wie Foren, Dateiablage etc. werden auch entsprechende dargestellt 
	und deren Einsatz und Nutzung betrachtet. Die Projektadministration wird im Vergleich zur Redmine Administration betrachtet, 
	um zu sehen welche M&ouml;glichkeiten ein Projektadministrator hat. Abschliessend ein Vergleich mit anderen Systemen wie z.B. 
	trac oder GForge runden die Betrachtung ab.</p>
	<a href="/files/LinuxTagBerlin2009Redmine.pdf" target="_blank">Redmine, das Projekt Management Werkzeug (PDF)</a>
	</li>
</ol>


<h2>Vortrag auf den Chemnitzer Linux Tagen 2009</h2>
<p>Entwicklung heute bedeutet auch immer eine &Uuml;bersicht &uuml;ber die Entwicklung zu haben, 
aber vor allem diese zu behalten. Das bedeutet, es muss ein entsprechendes Werkzeug 
eingesetzt werden, das das erm&ouml;glicht. </p>
<p>Im Rahmen des Vortrages wird die Projektmanagement-Software Redmine vorgestellt, 
die die genannte Aufgabe &uuml;bernehmen soll. Neben Installation, Nutzung und 
Konfiguration werden auch die Vor- und Nachteile von Redmine erl&auml;utert.</p>
<a href="/files/RedmineCLT2009.pdf" target="_blank">Redmine the project management tool (PDF)</a>


<h2>Vortrag auf den Chemnitzer Linux Tagen 2009 (Projektk&uuml;che)</h2>
<p>Im Rahmen der <a href="http://chemnitzer.linux-tage.de/2009/service/linux-nacht.html">Linux Nacht</a> hatte 
ich netterweise die Gelegenheit, das Open Source Projekt <a href="http://www.supose.org">SupoSE</a> vorstellen zu d&uuml;fen.</p>

<a href="/files/SupoSE-Short-CLT2009.pdf" target="_blank">The Subversion Repository Search Engine (SupoSE) (PDF)</a>

<h2><a href="http://2008.subconf.de/">Vortr&auml;ge auf der zweiten Subversion Conference 2008</a></h2>
<p>Im Rahmen des <a href="http://2008.subconf.de/powertrack-subversion/">Powertrack Subversion</a> habe ich auf der 
Subversion Conference 2008 in M&uuml;nchen 
insgesamt vier Vortr&auml;ge gehalten.</p>
<ol>
<li><h3><a href="http://2008.subconf.de/powertrack-subversion/karl-heinz-marbaise-iii/">Branching Strategien in der Software Entwicklung</a></h3>
	<p>Die Anwendung von Branching Strategien wird oft aus Unkenntnis vernachl&auml;&szlig;igt.
	Mithilfe von entsprechenden Strategien kann man das Projektmanagement
	unterst&uuml;tzen oder z.B. die Entkopplung von Entwicklung und Deployment
	erreichen.  Ein weiterer wichtiger Punkt ist die M&ouml;glichkeit, eine
	Qualit&auml;tsverbesserung zu erreichen.  Typische Indikatoren, die f&uuml;r den Einsatz
	solcher Strategien sprechen, ist das wiederholte auftauchen von Fehlern, die
	bereits in einer &auml;lteren Version beseitigt wurden.  Ein Punkt, der an
	Wichtigkeit zunimmt, ist die Kommunikation mit dem Kunden, da heute oft auch
	f&uuml;r Kunden entwickelt wird, die selbst eine Softwareentwicklung besitzen, die
	auf den eigenen Ergebnissen aufsetzt. Welche Release hat der Kunde? Welche Bugs
	wurden gel&ouml;st?  Welche Features wurden implementiert? etc.  Das sind typische
	Fragen, bei der eine entsprechende Branchingstrategie helfend zur Seite stehen
	und Unklarheiten beseitigen kann.  Im Rahmen der Anwendung von Branching
	Strategien ergeben sich meist auch Verbesserungen f&uuml;r die Bereiche Release-,
	Build-, Test- und Change-Management.</p>
	<a href="/files/SubConf2008BranchingStrategies.pdf" target="_blank">Branching Strategies (PDF)</a>
</li>
<li><h3><a href="http://2008.subconf.de/powertrack-subversion/karl-heinz-marbaise-iv/">Software Collaboration with OpenSource</a></h3>

	<p>Es gibt unterschiedliche Tools, um die Zusammenarbeit im Rahmen einer
	Softwarentwicklung zu verbessern. Dazu z&auml;hlen sog. Software Collaborations
	L&ouml;sungen. Hier sind aus dem Bereich OpenSource z.B. <a href="http://trac.edgewall.org">Trac</a>,
	<a href="http://www.redmine.org">Redmine</a>, <a href="http://gforge.org">GForge</a> zu
	nennen. Im Rahmen des Vortrags wird dargestellt, welche Vor- und Nachteile die
	einzelnen Werzeuge besitzen. Dazu z&auml;hlt beispielsweise die Installation und die
	Integration mit anderen Werkzeugen z.B.  mit der Versionskontrolle (z.B.
	Subversion).</p>

	<a href="/files/SubConf2008Collaboration.pdf" target="_blank">Software Collarboration with OpenSource (PDF)</a>
</li>

<li><h3><a href="http://2008.subconf.de/powertrack-subversion/karl-heinz-marbaise-i/">Hook'oholic &mdash; What can be done with hook scripts?</a></h3>
	<p>Subversion bietet mit den Hook-Scripten eine sehr flexible Schnittstelle, die
es erm&ouml;glicht, verschiedenste Pr&uml;fungen auf die &Uuml;bertragenen Daten zu
erm&ouml;glichen. Dabei sind die einfachsten; z.B. Pr&uuml;fung, ob die Log-Nachricht
eine bestimmte L&auml;nge hat oder einem bestimmten Format entspricht; nur die
Spitze des Eisberges.  Es besteht die M&ouml;glichkeit ein Berechtigungssystem
abseits vom Gebotenen zu entwickeln.  Weiterhin k&ouml;nnen bestimmte Pr&uuml;fungen auf
Properties etc. durchgef&uuml;hrt werden, um hier die M&ouml;glichkeit zu er&ouml;ffnen
verschieden Properties als obligatorisch zu definieren.</p>

	<a href="/files/SubConf2008HookScripts.pdf" target="_blank">Hook'oholic (PDF)</a>
</li>

<li><h3><a href="http://2008.subconf.de/powertrack-subversion/karl-heinz-marbaise-ii/">The pain of versions - Searching within one or more repositories</a></h3>
	<p>H&auml;ufig tritt das Problem auf, dass nach bestimmten Dateien oder Inhalten
	innerhalb von Subversion Repositories gesucht werden muss.  Mithilfe von
	vorhandenen Frameworks wie z.B. <a href="http://lucene.apache.org">Lucene</a>, <a href="http://www.opensymphony.com/quartz/">Quartz</a>, 
	<a href="http://www.svnkit.com">SVNKit</a> etc. ist es m&ouml;glich
	eine Suchmaschine zu erstellen, die mehrere Repositories scannt und die
	Inhalte zur Verf&uuml;gung stellt und somit eine Suche innerhalb von mehreren
	Repositories erm&ouml;glicht.  Damit ist es sehr einfach m&ouml;glich, Inhalte etc.
	einfach und schnell zu suchen. <a href="http://www.supose.org">SupoSE (Subversion Repository Search Engine)</a>
	bietet genau diese Funktionalit&auml;t.</p>
	<p>Sinn und Zweck ist es, die Suchmaschine und deren Konzept vorzustellen und
	auch, welche M&ouml;glichkeiten geboten werden und welche nicht. Hier w&auml;ren
	R&uuml;ckmeldungen der Besucher hilfreich, um zu sehen, welche Erweiterungen
	ben&ouml;tigt werden und welche nicht.</p>


	<a href="/files/SubConf2008SupoSE.pdf" target="_blank">SupoSE (PDF)</a>
</li>

</ol>


<h2><a href="http://2007.subconf.de/">Vortrag auf der ersten Subversion Conference 2007</a></h2>
<p>Der Vortrag behandelt die Nutzung, Konzepte und Installation von SVK, als 
Aufsatz auf Subversion zur verteilten Entwicklung. 
Hierbei werden die unterschiedlichen Konzepte zur Nutzung aufgezeigt und sowohl 
die Vor- als auch die Nachteile vorgestellt. Weiterhin werden im Rahmen des Vortages 
die unterschiedlichen Anwendungsf&auml;lle dargestellt. 
</p>
<a href="/files/SVKSubConf2007.pdf" target="_blank">Bringing Subversion to the next level? (PDF)</a>

<h2>Vortrag auf der Open Source Datenbank Conference 2006</h2>
<p>db4o die Alternative?</p>
<p>Die Nutzung von objekt orientierten Datenbanken ist bisher nicht
sehr popul&auml;r, wie auch immer, db4o stellt eine reale Alternative
zu normalen Datenbanken dar. Eine OO Datenbank die gleichzeitig noch eine
embedded Datenbank ist, kann sehr einfach genutzt werden und kommt 
ohne administrativen Aufwand aus. Die Application selbst und die 
Grenzen der Nutzen werden dargestellt.
</p>
<a href="/files/OSDBC2006db4o.pdf" target="_blank">db4o die Alternative? (PDF)</a>

<h2>Vortrag auf der PHP Conference 2006</h2>
<p>Business Integration von GForge per SOAP</p>
<p>
GForge ist ein Plattform, die eine Integration von Bug-Tracker, Wiki,
Issue-Tracking und Versionskontrolle bietet. Hier geht es um die Integration
von GForge per SAOP in Form eines "Proof of Concepts" in Richtung Java.
Dabei wird auf die Probleme im Bereich SOAP eingegangen und gezeigt,
wie einfach die Integration durch die Anwendung von SOAP wird.
</p>
<a href="/files/PHPCon2006BIGForge.pdf" target="_blank">Business Integration mit GForge (PDF)</a>

<h2>Vortrag auf der PHP Conference 2006</h2>
<p>Einfaches Testen von Webapplikationen mit SimpleTest</p>
<p>Anwendung und Nutzung von SimpleTest im Bereich des Testens von Webapplikationen.
Hierbei werden die M&ouml;glichkeiten und Grenzen von SimpleTest aufgef&uuml;hrt und einige
Beispiele zur Nutzung dargestellt. Es ist auch wichtig, die Testergebnisse in
Form von Reports zur Verf&uuml;gung zu stellen</p>

<a href="/files/PHPCon2006SimpleTest.pdf" target="_blank">SimpleTest (PDF)</a>

<h2>Vortrag auf der FrOSCon 2006</h2>
<p>In der Software Entwicklung werden Bug-Tracker, Wikis und Versionskontrollsysteme eingesetzt.
Das Problem ist, dass diese Komponenten meist alleine stehen und auch entsprechend genutzt werden.
Es ist aber wichtig und auch sinnvoll eine Kombination aller Kompontenen.
Das hei&szlig; t eine Verkn&uuml;pfung der Komponenten (Wiki, Bug-Tracker und Versionskontrollsystem).
Genau das macht Trac.
</p>
<a href="/files/TracFrOSCon2006.pdf" target="_blank">Software Collaboration mit Trac (PDF)</a>

<h2>Vortrag auf der FrOSCon 2006</h2>
<p>Die Verwendung von Subversion ist ja schon recht verbreitet,
aber was ist wenn man t&auml;glich unterwegs ist und keine oder nur eine
sporadische Verbindung mit einem Repository Server hat? Dann ist SVK das Werkzeug der Wahl.
</p>
<a href="/files/SVKFrOSCon2006.pdf" target="_blank">Verteiltes Versionsmanagement mit SVK (PDF)</a>

<h2>Vortrag auf den Chemnitzer Linux Tagen 2006</h2>
<p>Subversion erlangt immer mehr an Bedeutung auch im heimischen Bereich. Hier werden die
ersten Schritte vorgestellt, Erstellung eines Repositories, Import des ersten Projektes
in Subversion usw. Es wird auch auf die Installation von Subversion eingegangen.</p>
<a href="/files/EinfuehrungSubversion-ChemnitzerLinuxTage2006.pdf" target="_blank">Einf&uuml;hrung in Subversion (PDF)</a>

<h2>Vortrag auf der PHPConference 2005</h2>
<p>Das Testen von Web-Applikationen ist immer ein Problem und meist mit Aufwand
verbunden. Hier setzt die M&ouml;glichkeit an mithilfe von Web-Tests in Form von JWebUnit
den Test-Aufwand und die Pflege zu minimieren. Ein weiteres Ziel ist es solche Tests
zu automatisieren. Das kann durch die Anwendung mit Ant erreicht werden. Ein weiteres Problem
im Zusammenhang mit Web-Applikationen ist, dass meist immer Datenbank beteiligt sind.
Dafür gibt es aber auch L&ouml;sungen. Weitere Details k&ouml;nnen Sie im Vortrag nachlesen,
oder Sie treten einfach per EMail mit mir in Kontakt.</p>
<a href="/files/VortragPHPConference20051109.pdf" target="_blank">Welten vereinigt euch! Testen von PHP Applikationen mit Java Tools (PDF)</a>
