# Add to m2/settings.xml
	<server>
		<id>njb-nexus-snapshot</id>
		<username>admin</username>
		<password>admin123</password>
	</server>
	<server>
		<id>njb-nexus-release</id>
		<username>admin</username>
		<password>admin123</password>
	</server>
	
Advised to encrypt password using 
	mvn --encrypt-password
	
# Add to m2/settings.xml, for nexus group with maven central

	<mirrors>
	   <mirror>
			<id>central</id>
			<name>central</name>
			<url>http://localhost:9091/repository/njb-nexus-group/</url>
			<mirrorOf>*</mirrorOf>
		</mirror>
  	</mirrors>