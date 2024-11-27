This is branched from org.directwebremoting:dwr 3.0.3-SNAPSHOT.

To build,

edit version file in core/impl/main/java/dwr-version.properties

ant clean
ant jar

upload to nexus directly via web interface

file from dist/dwr-4.0.0-RELEASE.jar

groupId: com.forio.directwebremoting
artifactId: dwr
version: 4.0.0-RELEASE
classification: (blank)
packaging: jar

this command might also do it:
(not tested)

mvn deploy:deploy-file -DgroupId=org.directwebremoting -DartifactId=dwr -Dversion=4.0.0-RELEASE -Dpackaging=jar -Dfile=dist/dwr-4.0.0-RELEASE.jar  -Durl=https://dev.forio.com/nexus/content/repositories/releases -DrepositoryId=maven-releases


