# 地理公共库

主要包含了地理工具类、地理模型的实体类等

## 包介绍

* [constant](src/main/java/io/pifind/map/constant) : 常量包
* [model](src/main/java/io/pifind/map/model) : 地理模型实体类包
* [util](src/main/java/io/pifind/map/util) : 地理工具类包

## Maven 引入方式

**第一步** 请在 Maven 的 setting.xml 中添加如下服务器配置

```xml
<servers>
    <server>
      <id>pifind-maven-releases</id>
      <username>subscriber</username>
      <password>PiFind@2023$</password>
    </server>
    <server>
      <id>pifind-maven-snapshots</id>
      <username>subscriber</username>
      <password>PiFind@2023$</password>
    </server>
</servers>
```

**第二步** 在项目中增加 pifind 仓库

```xml
<repositories>
    <repository>
        <id>pifind-maven-releases</id>
        <url>https://pifind.mvn.pub/repository/maven-releases/</url>
    </repository>
    <repository>
        <id>pifind-maven-snapshots</id>
        <url>https://pifind.mvn.pub/repository/maven-snapshots/</url>
    </repository>
</repositories>
```

**第三步** 在项目的 pom.xml 中加入如下依赖

```xml
<!-- PiFind 公共仓库 -->
<dependency>
    <groupId>io.pifind.map</groupId>
    <artifactId>geo-common</artifactId>
    <version>0.0.1-snapshot</version>
</dependency>
```