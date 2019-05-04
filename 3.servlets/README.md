We will create a web application

    mvn archetype:generate -DgroupId={project-packaging} -DartifactId={project-name} -DarchetypeArtifactId=maven-archetype-webapp -DinteractiveMode=false

For my case the command is as below

    mvn archetype:generate -DgroupId=com.example -DartifactId=mywebapplication -DarchetypeArtifactId=maven-archetype-webapp -DinteractiveMode=false


Now create new static folder

    mkdir mywebapplication/src/main/resources/static

Create new file in above folder index.html

    <HTML>
        <HEAD>
            <TITLE>Your Title Here</TITLE>
        </HEAD>
        <BODY>
            This is static resource in HTML.
        </BODY>
    </HTML>


Now run this from folder mywebapplication

      mywebapplication>mvn clean package
 
This will generate war file at given location 
      
      target/mywebapplication.war 

Copy created war and copy in Tomcat installation webapp folder
After restart you should see Body message at URL
     
      http://localhost:8080/mywebapplicaton

    
