# Maven Commandline
1. Use this command to run class with Main method and main class specified in Pom:
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