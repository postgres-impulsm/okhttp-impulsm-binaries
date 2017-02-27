okhttp-impulsm-binaries
=======================


Using
-----

Insert to ``pom.xml`` (or to ``maven-settings.xml``):

    <dependencies>
      <dependency>
        <groupId>com.squareup.okhttp3</groupId>
        <artifactId>okhttp</artifactId>
        <version>20170227-IMPULSM-SNAPSHOT</version>
      </dependency>
    </dependencies>
    
    <repositories>
      <repository>
        <id>okhttp-impulsm-binaries</id>
        <!-- git@github.com:postgres-impulsm/okhttp-impulsm-binaries.git -->
        <url>https://raw.githubusercontent.com/postgres-impulsm/okhttp-impulsm-binaries/...GIT..TAG..NAME..HERE...</url>
      </repository>
    </repositories>


Develop
-------

Command to create local repository:

    cd ../okhttp/okhttp
    
    mvn install:install-file \
        -DlocalRepositoryPath='../../okhttp-impulsm-binaries' \
        -Dfile=target/okhttp-20170227-IMPULSM-SNAPSHOT.jar \
        -DpomFile=pom.xml \
        -DcreateChecksum=true
