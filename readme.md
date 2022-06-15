## Failed to execute goal org.apache.maven.plugins:maven-compiler-plugin:3.10.1:compile (default-compile) on project simple: Fatal error compiling: error: invalid target release: 17 -> [Help 1]
```
<build>
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
	</build>

```
```
<build>
		<plugins>
			<plugin>
				<groupId>org.apache.maven.plugins</groupId>
				<artifactId>maven-surefire-plugin</artifactId>
				<configuration>
					<forkCount>3</forkCount>
					<reuseForks>True</reuseForks>
					<argLine>-Xmx1024m -XX:MaxPermSize=256m</argLine>
				</configuration>
			</plugin>
		</plugins>
	</build>

```

##Failed to execute goal org.springframework.boot:spring-boot-maven-plugin:2.7.0:run (default-cli) on project simple: Application finished with exit code: 1 -> [Help 1]
```
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
            <plugin>
                <groupId>org.apache.maven.plugins</groupId>
                <artifactId>maven-compiler-plugin</artifactId>
                <version>3.8.0</version>
                <configuration>
                    <source>10</source>
                    <target>10</target>
                </configuration>
            </plugin>
``
