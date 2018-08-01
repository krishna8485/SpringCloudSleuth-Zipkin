# spring-cloud-Sleuth-Zipkin

Spring Cloud Zipkin and Sleuth Example


## Quick Start

Build code
git clone https://github.com/krishna8485/SpringCloudSleuth-Zipkin.git
cd SpringCloudSleuth-Zipkin


### Start Eureka Server

cd EurekaServer
gradle clean bootrun
Load http://localhost:8761/ to register the services.

### Start AddressService

cd AddressServer
gradle clean bootrun
Load http://localhost:8083/address
Use swagger-UI to invoke endpoint
http://localhost:8083/swagger-ui.html


### Start ZipCodeService

gradle clean bootrun
Load http://localhost:8084/zip/95616 

### Zipkin Server 

Download the Zipkin server from below link https://search.maven.org/remote_content?g=io.zipkin.java&a=zipkin-server&v=LATEST&c=exec

run the executable jar file using below command.

    java -jar zipkin-server-1.30.3-exec.jar

Once Zipkin is started, we can see the Web UI at http://localhost:9411/zipkin/.
