Maven创建的时候所需要的库文件

<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-web</artifactId>
		</dependency>
		
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-tomcat</artifactId>
			<scope>provided</scope>
		</dependency>
		<dependency>
			<groupId>org.apache.tomcat.embed</groupId>
			<artifactId>tomcat-embed-jasper</artifactId>
			<scope>provided</scope>
		</dependency>

		<dependency>
			<groupId>javax.servlet</groupId>
			<artifactId>jstl</artifactId>
		</dependency>
		<dependency>
			<groupId>org.slf4j</groupId>
			<artifactId>slf4j-api</artifactId>
			</dependency>
		<dependency>
			<groupId>ch.qos.logback</groupId>
			<artifactId>logback-core</artifactId>
			<version>1.1.2</version>
		</dependency>
		<dependency>
			<groupId>org.apache.httpcomponents</groupId>
			<artifactId>httpcore</artifactId>
			<version>4.3.2</version>
		</dependency>
		<dependency>
			<groupId>org.apache.httpcomponents</groupId>
			<artifactId>fluent-hc</artifactId>
			<version>4.3.3</version>
		</dependency>
		<dependency>
			<groupId>com.alibaba</groupId>
			<artifactId>fastjson</artifactId>
			<version>1.1.39</version>
		</dependency>
		<dependency>
			<groupId>commons-logging</groupId>
			<artifactId>commons-logging</artifactId>
			<version>1.2</version>
		</dependency>
		<dependency>
			<groupId>commons-io</groupId>
			<artifactId>commons-io</artifactId>
			<version>2.6</version>
		</dependency>
		<dependency>
			<groupId>org.apache.directory.studio</groupId>
			<artifactId>org.apache.commons.codec</artifactId>
			<version>1.8</version>
		</dependency>
		<dependency>
		<groupId>org.apache.maven.plugins</groupId>
		<artifactId>maven-surefire-plugin</artifactId>
		<version>2.12.4</version>
		</dependency>
		<dependency>
			<groupId>client-adpter</groupId>
			<artifactId>client-adapter-sdk-java-oauths-json</artifactId>
			<version>0.3.12</version>
		</dependency>
		<dependency>
			<groupId>org.apache.maven.plugins</groupId>
			<artifactId>maven-resources-plugin</artifactId>
			<version>2.4</version>
		</dependency>
		<dependency>
			<groupId>com.sun.jersey</groupId>
			<artifactId>jersey-server</artifactId>
			<version>1.18</version>
		</dependency>
		<dependency>
			<groupId>com.sun.jersey</groupId>
			<artifactId>jersey-grizzly2</artifactId>
			<version>1.18</version>
		</dependency>
		<dependency>
			<groupId>sae</groupId>
			<artifactId>sae-hr</artifactId>
			<version>1.1.3</version>
		</dependency>
		<dependency>
			<groupId>com.unboundid</groupId>
			<artifactId>unboundid-ldapsdk</artifactId>
			<version>3.2.1</version>
		</dependency>
		<dependency>
			<groupId>org.jsoup</groupId>
			<artifactId>jsoup</artifactId>
			<version>1.7.3</version>
		</dependency>
		<!--  <dependency>
			<groupId>qrcode</groupId>
			<artifactId>qrcode</artifactId>
			<version>1.0.29</version>
		</dependency>
		<dependency>
			<groupId>qrcoe</groupId>
			<artifactId>qrcode</artifactId>
			<version>1.0.729</version>
		</dependency>-->
	</dependencies>

	<properties>
		<java.version>1.8</java.version>
		<start-class>com.shiku.mianshi.Application</start-class>
		<main.basedir>${basedir}/../..</main.basedir>
		<m2eclipse.wtp.contextRoot>/</m2eclipse.wtp.contextRoot>
	</properties>

	<!-- Package as an executable jar -->
	<build>
		<plugins>
			<plugin>
				<groupId>org.springframework.boot</groupId>
				<artifactId>spring-boot-maven-plugin</artifactId>
				<version>1.1.6.RELEASE</version>
				<executions>
					<execution>
						<goals>
							<goal>repackage</goal>
						</goals>
					</execution>
				</executions>
			</plugin>
			<plugin>
				<groupId>org.apache.maven.plugins</groupId>
				<artifactId>maven-compiler-plugin</artifactId>
				<version>2.3.2</version>
				<configuration>
					<source>1.8</source>
					<target>1.8</target>
					<encoding>UTF-8</encoding>
				</configuration>
			</plugin>
		</plugins>
	</build>
