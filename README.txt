=======================
Elastic Search Tutorial
=======================
2015-11-06 Fri 09:20 AM
Playing around with Elastic Search on Windows.

References
==========
Following steps from the elasticsearch getting started video:
http://p.brightact.com/p/showTile/10137

Elastic search setup guide
https://www.elastic.co/guide/en/elasticsearch/reference/current/setup.html

Steps 1-5
https://www.youtube.com/watch?v=l6wXE5SBJ_A

Steps
=====

1. Extract from folder. This is the first commit.
2. Change configuration variables
3. Download Java JDK

http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html
instructions - basically download/install and change windows path:
http://docs.oracle.com/javase/8/docs/technotes/guides/install/windows_jdk_install.html#chdebccj

4. Set JAVA_HOME environment variable to C:\Program Files\Java\jdk1.8.0_65
http://www.wikihow.com/Set-Java-Home

5. Run bin/elasticsearch.bat

6. go to http://localhost:9200/ in your browser.

The video suggests to use curl, which isn't on windows.
Also try
http://localhost:9200/_cluster/health
http://localhost:9200/_cluster/health?pretty

7. Install Marvel. It's a Browser-based UI for elasticsearch.
The video says
Windows: plugin install elasticsearch/marvel/latest
Linux: plugin -i elasticsearch/marvel/latest

It couldn't find it. Instead, from 
https://www.elastic.co/guide/en/marvel/current/installing-marvel.html

Windows, in elasticsearch-2.0.0/bin directory: 
plugin install license
plugin install marvel-agent

8. Install Kabana. I'm not sure what it is.
https://www.elastic.co/downloads/kibana

9. Set the elasticsearch.url to the elasticsearch instance.
