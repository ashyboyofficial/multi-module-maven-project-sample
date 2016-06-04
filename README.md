# multi-module-maven-project-sample

This application is a stub project of multi module maven project.

The idea behind having a multi-module project is to separete out the application features or modules. These features/modules are to be implemented in separate project under a parent project.

Parent project consists of a single POM. This POM acts as a parent POM for all the POMs in the child project.
Parent POM holds the information of all the child projects as shown below.

```xml
<modules>
		<module>../mm-module1</module>
		<module>../mm-module2</module>
		<module>../mm-module3</module>
		<module>../mm-web</module>
</modules>
```

So, when we execute a maven build, it builds all the child projects and creates the artifacts mentioned in the POM.

Following is the structure of the multi-module project.

![alt tag](https://raw.githubusercontent.com/ashyboyofficial/multi-module-maven-project-sample/master/resource/project.jpg)
