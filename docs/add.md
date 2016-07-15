# add maven to java project in eclipse

## References
* http://stackoverflow.com/questions/7139560/convert-existing-project-to-a-maven-project

##### Add the m2e plugin
* Window > Preferences > Install/Update > Available Software Sites > Add
  * Name: Maven
  * Location: http://download.eclipse.org/m2e-wtp/releases/
* Help > Install New Software
  * Work with: Maven
    * Select Maven Integration for Eclipse
    * Click Next
    * Click Next
    * Accept the license agreement
    * Restart

##### Move your code into the src/main/java folder

##### Move your unit tests to src/test/java

##### DO NOT copy your libraries & jars

##### Check all the compilation errors caused because of the missing jars

##### Add dependency of each missing jar to pom.xml. 
* You can get the dependency from the maven repository websites. 
* If you have already indexed the repositories in m2e plugin, then you can simply search of the dependency within the plugin and add it from right there.
