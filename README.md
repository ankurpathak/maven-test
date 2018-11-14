# Maven Commandline
1. Use this command to run class with Main method and with class specified in Pom:
```
        mvn exec:java
```
2. If plugin goal tied with package phase of default maven life cycle by:
```
        <executions>
            <execution>
                <id>my-execution</id>
                <phase>package</phase>
                <goals>
                    <goal>java</goal>
                </goals>
            </execution>
        </executions>
```

then use command to run:
```
        mvn package
```
3. Run class with Main method directly with command:
```
         mvn exec:java -Dexec.mainClass=com.github.ankurpathak.HelloWorld
```
4. With shade plugin used to package application as uber jar, use
following command to run application:
```
        mvn package
        java -jar application.jar
```
