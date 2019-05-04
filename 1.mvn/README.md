You can change your application by replacing com.example
ArtifactId can also be modified based on your requirement

    mvn archetype:generate -DgroupId=com.example -DartifactId=myapplication -DarchetypeArtifactId=maven-archetype-quickstart -DarchetypeVersion=1.4 -DinteractiveMode=false

Now this will generate folder of name same as artifactId

    cd myapplication

Now we can look into how maven works and what it does
    mvn dependency:tree


