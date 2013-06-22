---
layout: post
title: "SupoSE Release 0.6.2 Calypso ist nun da"
date: 2010-06-11 18:59:57
tags: SKM,Neue Versionen,Subversion,SupoSE
categories: SKM,Neue Versionen,Subversion,SupoSE
post-type: blog
---
Eine neue Release von <a href="http://www.supose.org/wiki/supose">SupoSE</a> ist nun fertig. 

<ul>
   <li>User visible Changes/Enhancements.
      <ul>
          <li>Upgrade to SVNKit 1.3.X (Support for SVN 1.6.X repositories) (#218)</li>
          <li>Enormous performance enhancements for the scan command (#309)</li>
          <li>Updated to Java 1.6 (#235)</li>
          <li>Removed the dfilename and dpath which had been introduced in Release 0.6.0 to reduce the Index size finger print (#241).</li>
          <li>Removed display property prefix (#310)</li>
          <li>Output formatting of --help has been changed (#36)</li>
          <li>quartz.properties are now located in the etc folder</li>
          <li>Formatting problem if more than 9999 items in changeset (#314)</li>
          <li>Copyright updated to 2010 (#308)</li>
          <li>Updated the Build/Run Documentation (#247)</li>
      </ul>
   </li>
   <li>Fixed Bugs
       <ul>
          <li>Fuzzy search had been broken (#199)</li>
          <li>README will not correctly recognized (#215)<li>
          <li>Searching for full qualified filenames didn't work (#216)<li>
          <li>Couldn't search for files with a dot (#246)</li>
        </ul>
    </li>
    <li>Won't be fixed:
       <ul>
          <li>Support for 1.1.X Repositories which fails with SVNKit (#34, #141)</li>
        </ul>
    </li>
    <li>Build Changes
       <ul>
          <li>Fixed missing dependencies for bouncycastle which is needed for PDF files (#250)</li>
          <li>Analyzed the dependencies in Maven build (#225)</li>
          <li>Updated to Tika 0.4, 0.5, 0.6, 0.7 (#219, #239, #266, #304)</li>
          <li>Updated to ANTLR3 Maven Plugin (#201, #298)</li>
          <li>Updated to SVNKit 1.3.1 (#218)</li>
          <li>Updated Quartz Scheduler to 1.7.3 (#303)</li>
          <li>Update Maven License Plugin from 1.5.0 to 1.6.1 (#311)</li>
          <li>NoSuchElementException during Site build (#300)</li>
          <li>problem in generated documentation (#301)</li>
          <li>Checked compatibility with Maven 3-beta-1</li>
       </ul>
     <li>Other changes
         <ul>     
            <li>Fixed Comments for revisions r439-r441 (#259)</li>
         </ul>
      </li>
      <li>Known Limitations
          <ul>
          <li>At the moment the Job Scheduler does not contain the performance improvements (#309)</li>
          </ul>
      </li>
</ul>
<br/>

Das <a href="http://www.supose.org/attachments/download/60/supose-0.6.2-bin-unix.tar.gz">Unix binary</a> lÃ¤uft auf Linux als auch auf Mac OS X. FÃ¼r <a href="http://www.supose.org/attachments/download/59/supose-0.6.2-bin.zip">Windows</a> ist selbstverstÃ¤ndlich auch gesorgt.