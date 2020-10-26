## 快速开始

**安装到本地仓库**

```shell
mvn clean install
```

**更新本地仓库的`archetype-catalog.xml`**

```shell
mvn archetype:update-local-catalog
```

**创建项目**

```shell
mvn archetype:generate -D interactiveMode=false \
                       -D archetypeCatalog=local \
                       -D archetypeGroupId=xyz.icefery.archetypes \
                       -D archetypeArtifactId=maven-archetype-webapp \
                       -D archetypeVersion=1.0.0 \
                       -D groupId=xyz.icefery.demos \
                       -D artifactId=demo1 \
                       -D version=0.0.1-SNAPSHOT \
                       -D package=xyz.icefery.demos.demo1
```

> 原型`package`的默认值为`${groupId}.artifactid`，若不指定，创建项目后需手动修改。

