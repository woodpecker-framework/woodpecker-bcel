# woodpecker定制版BCEL编码库

## 0x01 简介
该代码是从JDK7u21中提取，并简单开发而成。为的是解决在JDK某些版本BCEL被剔除，导致使用BCEL编码的插件报错问题。

推荐编写woodpecker插件全部使用该库，去除jdk的依赖。

## 0x02 使用

#### 编码

```java
HackBCELs.encode("/tmp/Test.class");
```

#### 解码

```java
String strBCEL = "$$BCEL$$...";
HackBCELs.decode(strBCEL);
```