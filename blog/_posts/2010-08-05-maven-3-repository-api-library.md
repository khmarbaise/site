---
layout: post
title: "Maven 3 - Repository API Library"
date: 2010-08-05 08:45:30
tags: Neuigkeiten,BM,Maven
categories: Neuigkeiten,BM,Maven
post-type: blog
---
Im <a href=" http://www.sonatype.com/people/2010/08/introducing-aether/">Sonatype Blog</a> ist zu lesen, dass es jetzt eine unabhÃ¤ngige Library gibt, um den <a href="https://docs.sonatype.org/display/COMM/Repository+API+for+Maven+3.x">Repository Zugriff aus Maven 3</a> verwenden zu kÃ¶nnen ohne Maven vollstÃ¤ndig inkl. Plexus einzubinden zu mÃ¼ssen. Das bedeutet hier Ã¶ffnen sich TÃ¼ren, um weitere Tools aufbauend darauf zu erstellen. Das bedeutet auch, dass die Infrastruktur wie z.B. Maven Repositories (z.B. verwaltet mit einem Nexus Repository Manager o.Ã¤.) als Grundlage zur AuflÃ¶sung von AbhÃ¤ngigkeiten in anderen Applikationen und Anwendungen nutzbar werden. Der <a href="http://github.com/sonatype/sonatype-aether">Source ist via github</a> zu beziehen.