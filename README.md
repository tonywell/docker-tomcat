# Tomcat Docker镜像

### 构建Image

通过默认参数构建基于java7的tomcat7镜像

```
$ docker build -t tonywell/tomcat -f jdk7/Dockerfile .
```

通过默认参数构建基于java8的tomcat8镜像

```
$ docker build -t tonywell/tomcat -f jdk8/Dockerfile .
```

使用参数指定tomcat版本构建镜像

- TOMCAT_MAJOR_VERSION：7 or 8 or 9
- TOMCAT_UPDATE_VERSION: The minor version from any tomcat download page.
- TOMCAT_BUILD_NUMBER: The build number from any tomcat download page.

Example:

```
$ docker build -t tonywell/tomcat \

  --build-arg TOMCAT_MAJOR_VERSION=8 \

  --build-arg TOMCAT_UPDATE_VERSION=5 \

  --build-arg TOMCAT_BUILD_NUMBER=9 \

  -f jdk7/Dockerfile .

```

构建基于jdk7的tomcat8.5.9的镜像，基于jdk8的同理。