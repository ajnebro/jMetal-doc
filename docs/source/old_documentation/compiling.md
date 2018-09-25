## Compiling

Once you have the source code of jMetal you can use it in to ways: from an IDE or from the command line of a terminal. The IDE alternative is the simplest one and, if you are used to the tool, compiling and running algorithms is easy.

### Intellj Idea
  To build the project you have to select `Build` -> `Make Project`
  
![Building with IntelliJ Idea](https://github.com/jMetal/jMetalDocumentation/blob/master/figures/BuildIJICE14.png)  
  
  
###Eclipse
  If the `Project` -> `Build Automatically` is set, Eclipse will automatically build the project. Otherwise,  select  `Project` -> `Build Project`
  
![Building with Eclipse](https://github.com/jMetal/jMetalDocumentation/blob/master/figures/BuildEclipse.png)  

  
###Netbeans:
  In Netbeans you have to select `Run` -> `Build Project`

![Building with Netbeans](https://github.com/jMetal/jMetalDocumentation/blob/master/figures/BuildNetbeans.png)  

### Building from the command line

Once you have downloaded the source code you can use the command line to build the project by using Maven commands. If you open a terminal you will have something similar to this:

![jMetal in a terminal](https://github.com/jMetal/jMetalDocumentation/blob/master/figures/jMetalInTerminal.png)  

Then you have Maven to your disposal to work with the project:
* `mvn clean`: cleaning the project
* `mvn compile`: compiling
* `mvn test`: testing
* `mvn package`: compiling, testing, generating documentation, and packaging in jar files
* `mvn site`: generates a site for the project
