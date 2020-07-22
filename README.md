# Managing Your Google Cloud Infrastructure
This file contains text you can copy and paste for the examples in Cloud Academy's _Managing Your Google Cloud Infrastructure_ course.  

### Introduction
[Free GCP Trial](https://cloud.google.com/free) 

### Monitoring
[Installing the Cloud Monitoring agent](https://cloud.google.com/monitoring/agent/install-agent)  
[Installing the Cloud Logging agent](https://cloud.google.com/logging/docs/agent/installation)

### Logging
```
select * from example_dataset.syslog_<date> WHERE textPayload LIKE '%shutdown%'
```

### Error Reporting and Debugging
[Google Cloud SDK](https://cloud.google.com/sdk)  
[Java SE 11 Development Kit](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html)  
[Git](https://git-scm.com/downloads)  
[Maven 3.5 or greater](https://maven.apache.org/download.cgi)  

```
git clone https://github.com/GoogleCloudPlatform/java-docs-samples
cd java-docs-samples/appengine-java11/springboot-helloworld
mvn spring-boot:run
gcloud app deploy
```
```
int bad = 1/0;
```
```
    String osname = System.getProperty("os.name");
    if (osname.equals("Ubuntu"))
      return "Ubuntu rocks!";
    else
      return "Hello world!";
```
```
    if (osname.equals("Linux"))
      return "Linux rocks!";
````
