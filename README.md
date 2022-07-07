# snowflake-connectivity

Json Logger

https://github.com/mulesoft-consulting/json-logger

If go to json-logger/template-files   open settings.xml

will find  Exchange2  under server  add anypoint platform credentials

sameway change the anypoint platform credentials under exchange2 of serever in .m2 settings.xml

open json-logger  

open gitbash here and enter below command

./deploy-to-exchange.sh 1ff09320-849e-466f-bc92-be792e06cfef

/////////////////////////////////////////////



Building Common project utility Jar


Dependency of ur pom:

<dependency>
			<groupId>ur groupID</groupId>
			<artifactId>ur ArtificatId</artifactId>
			<version>ur Version</version>
		</dependency>
  First run the maven command and build the jar it will create target folder
  After run the below command inside the target folder it will compress to packaging jar
  

Run the Below command

mvn install:install-file -Dfile=snowflake-connectivity-1.0.0-SNAPSHOT-mule-application.jar  -DgroupId=com.mycompany  -DartifactId=snowflake-connectivity  -Dversion=1.0.0-SNAPSHOT -Dpackaging=jar


Once successfully run the command add dependency,shared libraries of jms,snowflake  in pom.xml in your calling project
Next Go to calling project In Global Elements import ur common utility configuration.xml file once added successfully
we can able to access the common utility by using flow reference to call the flows.



