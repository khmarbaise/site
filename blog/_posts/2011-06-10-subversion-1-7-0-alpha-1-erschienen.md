---
layout: post
title: "Subversion 1.7.0 Alpha 1 erschienen"
date: 2011-06-10 19:22:16
tags: 
categories: 
post-type: blog
---
Die erste Alpha Release von <a href="http://old.nabble.com/Apache-Subversion-1.7.0-alpha1-Released-ts31818310.html">Subversion 1.7 Alpha 1</a> ist erschienen. <a href="http://subversion.apache.org/docs/release-notes/1.7.html">Was gibt es denn so neues?</a> Tja vor allem ein vÃ¶llig neues Working Copy Format. Das heiÃŸt zum einen checkout's die bis dato existieren werden von einem SVN Client nicht upgedated. Das bedeutet dass die Working Copies neu ausgecheckt werden mÃ¼ssen. Es gibt auch keine mÃ¶glichkeit eines upgrades der working copy. Das neue Working Copy format ist vor allem in der Hinsicht einfacher und besser, dass nicht in jedem Unterverzeichnis ein ".svn" Verzeichnis besitzt sondern nur noch auf der obersten Ebene (Ã¤hnlich wie Git, Mercurial, Bazaar etc.). Das bedeutet eine Performance Verbesserung im Bezug auf die Working Copy (vor allem bei groÃŸen). Weiterhin ein interessanter Aspekt ist, dass die Kommunikation im Falles eines 1.7 Servers mit dem neuen HTTPv2 Protokolll lÃ¤uft. Die genaue Liste der Ã„nderungen kann man im <a href="http://svn.apache.org/repos/asf/subversion/trunk/CHANGES">ChangeLog</a> nach lesen..