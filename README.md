# JAVA JAR APP buildpack

云帮为了让您更方便的部署项目，特推出可识别**JAR包**的构建模式- **JAVA JAR APP buildpack** 。

## 工作原理

当buildpack在您的代码根目录检测到 `LANGUAGE` 文件，并且内容为 `java-jar`，该应用被识别为JAR项目。我们称为Java-jar。

## 文档

以下文章了解更多：

- [云帮支持Java](https://www.rainbond.com/docs/stable/user-lang-docs/java/lang-java-overview.html)
- [云帮部署JAR包应用](https://www.rainbond.com/docs/stable/user-lang-docs/java/lang-java-maven.html)

## 配置

### 默认环境

buildpack构建环境默认使用 **JDK1.8** 版本。

### Procfile文件内容

```
web: java -cp config/:lib/*.jar:bin/.class Example
```

请根据目录的实际情况写`Procfile` 的内容

## 授权

根据 MIT 授权证获得许可。 请参阅LICENSE文件
