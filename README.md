# woodpecker定制版BCEL编码库

## 0x01 简介
该代码是从`JDK7u21`中提取，并简单开发而成。**为的是解决在JDK某些版本BCEL被剔除，导致使用BCEL编码的插件报错问题。**

推荐编写woodpecker插件全部使用该库，去除jdk的依赖。

## 0x02 使用

```
<dependency>
  <groupId>me.gv7.woodpecker</groupId>
  <artifactId>woodpecker-bcel</artifactId>
  <version>0.1.0</version>
</dependency>
```

#### 2.1 编码

```java
HackBCELs.encode("/tmp/Test.class");
```

#### 2.2 解码

```java
String strBCEL = "$$BCEL$$...";
HackBCELs.decode(strBCEL);
```
