Apache Maven 3.9.12

Maven home: D:\Programs\maven

Java version: 1.8.0_451, vendor: Oracle Corporation, runtime: D:\Programs\jdk1.8.0_451\jre

M2_HOME: D:\Programs\.m2\repository

-- jbpm documentation portal

https://docs.jbpm.org/latest/jbpm-docs/html_single/

-- Business Applications - Getting Started

https://kie.apache.org/docs/components/jbpm/getting_started/

-- Go to below folder

D:\Code\eclipse-2024-09-4330\rhpamapp2

-- Run below three mvn project creation commands

mvn archetype:generate -B -DarchetypeGroupId=org.kie -DarchetypeArtifactId=kie-model-archetype -DarchetypeVersion=7.74.1.Final -DgroupId=com.company -DartifactId=business-application-model -Dversion=1.0-SNAPSHOT -Dpackage=com.company.model

mvn archetype:generate -B -DarchetypeGroupId=org.kie -DarchetypeArtifactId=kie-kjar-archetype -DarchetypeVersion=7.74.1.Final -DgroupId=com.company -DartifactId=business-application-kjar -Dversion=1.0-SNAPSHOT -Dpackage=com.company

mvn archetype:generate -B -DarchetypeGroupId=org.kie -DarchetypeArtifactId=kie-service-spring-boot-archetype -DarchetypeVersion=7.74.1.Final -DgroupId=com.company -DartifactId=business-application-service -Dversion=1.0-SNAPSHOT -Dpackage=com.company.service -DappType=bpm

-- YouTube video for reference

https://www.youtube.com/watch?v=tV5_uyyNwUk 

-- Run launch script, to do mvn clean install, BUT IT FAILS TO START THE APP

D:\Code\eclipse-2024-09-4330\rhpamapp2\business-application-service> launch.bat clean install 

-- Create multi module maven project and add above created 3 projects to it

-- Update parent pom to use spring-boot-starter-parent as it parent

-- Run launch script, to do mvn clean install, IT WORKS

D:\Code\eclipse-2024-09-4330\rhpamapp2\business-application-service> launch.bat clean install 

http://localhost:8090/

http://localhost:8090/rest/server

