## 快速开始

**安装到本地仓库**

```shell
mvn clean install
```

**在本地仓库更新（生成）`archetype-catalog.xml`**

```shell
mvn archetype:update-local-catalog
```

**通过原型创建项目**

```shell
mvn archetype:generate -D interactiveMode=false \
                       -D archetypeCatalog=local \
                       -D archetypeGroupId=xyz.icefery.archetypes \
                       -D archetypeArtifactId=maven-archetype-webapp \
                       -D archetypeVersion=0.0.1 \
                       -D groupId=xyz.icefery.tests \
                       -D artifactId=test1 \
                       -D version=0.0.1 \
                       -D package=xyz.icefery.tests.test1
```

