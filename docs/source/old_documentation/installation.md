<!--<div id='id-installation'/>-->
## Installation
jMetal is a Maven project hosted in GitHub, so there are two ways of getting the software: adding it as a dependence in your own Maven project, or getting the source code from https://github.com/jMetal/jMetal.

### Using jMetal as a Maven/Gradle dependence
jMetal 5 is structured into four submodules:
* `jmetal-core` : Classes of the core architecture plus some utilities, including quality indicators.
* `jmetal-algorithm` : Implementations of metaheuristics.
* `jmetal-problem` : Implementations of problems.
* `jmetal-exec` : Executable programs to configure and run the algorithms plus some utilities.

These modules can be found in the [Central Repository](http://search.maven.org/) (note that the last version is jMetal 5.6):
![jMetal in Central Repository](https://github.com/jMetal/jMetalUserManual/blob/master/figures/centralRepository.png)

Here you can get the Maven dependency you need. For example, if your want to use some of the classes in `jmetal-core`, you just have to add this dependence to the `pom.xml` file of your project:
![Maven dependence](https://github.com/jMetal/jMetalUserManual/blob/master/figures/mavenDependence.png)

For Gradle the process is similar. Make sure you have the Maven repository listed in your build.gradle:

```Groovy
repositories {
    mavenCentral()
}
```

You can then use the same modules as for Maven. For example to add a dependency to the core and algorithm modules:

```Groovy
dependencies {
    compile (
            [group: 'org.uma.jmetal', name: 'jmetal-core', version: '5.2'],
            [group: 'org.uma.jmetal', name: 'jmetal-algorithm', version: '5.2']
    )
}
```

The same can be done in case of need the other packages.

### Getting the source code from GitHub
And advantage of having a project in GitHub is that you can easily get a copy of the source code just by cloning it. This can be done in several ways:
* Using Git from the command line of a terminal:
```
git clone https://github.com/jMetal/jMetal.git
```
* Selecting the button "Clone in Desktop" that is located in the right side of the page in https://github.com/jMetal/jMetal
* Alternatively, you can download a Zip file with all the files by pushing the button "Download ZIP" in the same page

Once you have the source code, you use you favorite IDE to import (Eclipse) or open (Intellij Idea) the project as a Maven project, or merely open it (Netbeans).
