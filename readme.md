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
