Tinker Modular Struts 2 Archetype
--------------------------------------------------------------------------------
If you're reading this then you've created your new project using Maven and
tinker.  You have only created the shell of an AppFuse Java EE
application.  The project object model (pom) is defined in the file pom.xml.
The application is ready to run as a web application. The pom.xml file is
pre-defined with Hibernate as a persistence model and Struts 2 as the web
framework.

There are two modules in this project. The first is "core" and is meant to 
contain Services and DAOs. The second is "web" and contains any web-related
files. Using this modular archetype is recommended when you're planning on
using "core" in multiple applications, or you plan on having multiple clients
for the same backend.

To get started, complete the following steps:

1. Download and install a MySQL 5.x database.

2. From the command line, cd into the core directory and run "mvn install".

3. From the command line, cd into the web directory and run "mvn jetty:run".

   remark：（1）In order to facilitate the development, you can use Tomcat. 
                Only need to convert web engineering works
           （2）IF jetty：run Persistent PermGen OutofMemory Error you can set
 		        my MAVEN_OPTS（mvn or javeEE）environment variable to the following:
                
				-Xmx1024M -XX:PermSize=512m -XX:MaxPermSize=1024m -Djava.awt.headless=
				true -XX:+CMSClassUnloadingEnabled -XX:+UseConcMarkSweepGC

4. View the application at http://localhost:8080.

5. Tinker Project Base on AppFuse，More information can be found at:

    http://appfuse.org/display/APF/AppFuse+QuickStart
	
6. If you have questions you can visit My Blog，My Blog is：

    http://blog.csdn.net/cloudyxuq	
	

