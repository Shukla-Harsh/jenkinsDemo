Envrioment setup instructions: You'll need JDK, maven and an IDE to run this project locally.

Download and install a JDK
Jenkins is based on Java, so to build Jenkins plugins you need to install a Java Development Kit (JDK). Recent Jenkins releases require JDK 8 to run, so that’s what we’re using in this tutorial.

You can download and install JDK 8 from the Oracle website.

Download and install Maven
Jenkins plugins mostly use Maven to build, so that’s what we’re going to use in this tutorial.

Download Maven from Apache Maven website. Make sure to download one of the binary files (with bin in their name).

Extract Maven, and take note of its location. Then, add the the full path of the bin/ subdirectory extracted (for example, ~/Applications/apache-maven/bin/mvn or C:\Program files\Maven\bin\mvn) to the PATH variable in your OS. (This will let you invoke Maven using mvn).

To verify that Maven is installed, run the following command:

mvn -version

IntelliJ IDEA
We are using intellij to develop/maintain this project. Please download/install Intellij. Make sure you also add the full path of bin folder(C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2021.1.2\bin for me) to the PATH variable.

Check out and start your Jenkins
Check out this branch locally. Go to your local branch(C:\Hackathon2021\JenkinsIdentifyMe\identify-me-jenkins in my case). Start command line tool/terminal from this directory and run the following command.

idea64 pom.xml

Now intellij should import your project as a Maven project.

In intellij, go to File -> Project Structure -> Project -> Project SDK. Select your 1.8 SDK then click 'OK'.

Now go to terminal in intellij and run the following two commands.

mvn verify

mvn hpi:run

Once you run these two successfully, your Jenkins is up and running. You can go to the following url to check.

http://localhost:8080/jenkins/
