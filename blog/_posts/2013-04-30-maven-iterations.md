---
layout: post
title:  "Iterations and Maven? Not possible?"
date:   2013-05-18 18:39:28
tags:   Maven, iterator-maven-plugin
categories: Build Management, Maven
post-type: blog
---

During my experiences with Maven I had a few moments where I wished 
having some kind of iterations to go over a list of whatever (servers, 
environments etc.). After some thinking about the problem i have 
decided to write my own plugin which will solve the problem. And now I 
have created such [plugin][github-iterator-maven-plugin]. Currently the
 plugin can be used by using it from the [staging repository][oss-staging-repository]
After some feedback i will release it to Maven central. If you find 
some problems with the plugin you can create a [ticket on github][github-iterator-maven-plugin-issues]
or write an <a href="mailto:mavenplugin@soebes.de">email to me</a>. You 
can use the plugin like the following:

In this case it will iterator over the given list test,prod and dev and 
call for every item the [maven-assembly-plugin][maven-assembly-plugin]. 
The following code:

{% highlight xml linenos %}
<plugin>
  <groupId>com.soebes.maven.plugins</groupId>
  <artifactId>iterator-maven-plugin</artifactId>
  <version>0.1.0</version>
  <executions>
    <execution>
      <phase>package</phase>
      <goals>
        <goal>executor</goal>
      </goals>
      <configuration>
        <items>
          <item>test</item>
          <item>prod</item>
          <item>dev</item>
        </items>
 
        <pluginExecutors>
          <pluginExecutor>
            <plugin>
              <groupId>org.apache.maven.plugins</groupId>
              <artifactId>maven-assembly-plugin</artifactId>
              <version>2.4</version>
            </plugin>
            <goal>single</goal>
            <configuration>
              <descriptors>
                <descriptor>${project.basedir}/<sub>item</sub>.xml</descriptor>
              </descriptors>
            </configuration>
          </pluginExecutor>
        </pluginExecutors>
      </configuration>
    </execution>
  </executions>
</plugin>
{% endhighlight %}

If you need you can execute several plugins as well. Just use an 
extra pluginExecutor for each of your plugins. So in other words: 
Iteration or foreach in Maven is solved.

