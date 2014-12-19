Spring Boot with Maven and Docker
========================
Part of the blog post: http://blog.adaofeliz.com/2014/11/21/first-look-spring-boot-and-docker

Installation
--------------
* Clone this project
```sh
git clone https://github.com/corradolupo/spring-boot-maven-docker.git spring-boot
```

* Build Application
```sh
cd spring-boot
mvn clean install
cd target
docker build -t spring-boot .
```

* Deploy to Docker Container
```sh
docker images
docker run -p 8080:8080 <image id>
```

Try it
--------------
- Now open your browser: http://localhost:8080/

License
--------------
MIT
