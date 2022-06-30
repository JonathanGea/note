## Failed to execute goal org.springframework.boot:spring-boot-maven-plugin:2.7.0:run (default-cli) on project simple: Application finished with exit code: 1 -> [Help 1]
ganti port yang belum digunakan
```
 <plugins>
            <plugin>
                <groupId>org.springframework.boot</groupId>
                <artifactId>spring-boot-maven-plugin</artifactId>
                <configuration>
                    <excludes>
                        <exclude>
                            <groupId>org.projectlombok</groupId>
                            <artifactId>lombok</artifactId>
                        </exclude>
                    </excludes>
                </configuration>
            </plugin>
   </plugins>
```

## Failed to execute goal org.apache.maven.plugins:maven-compiler-plugin:3.10.1:compile (default-compile) on project simple: Fatal error compiling: error: invalid target release: 17 -> [Help 1]
comment version of java in pom.xml

```
<properties>
		<!--<java.version>17</java.version>-->
		<spring-cloud.version>2021.0.3</spring-cloud.version>
	</properties>
```
