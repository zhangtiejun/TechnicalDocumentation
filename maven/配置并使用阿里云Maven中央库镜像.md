# 配置并使用阿里云Maven中央库镜像

标签（空格分隔）： maven mirror central 阿里云 镜像

---

为了提高从Maven服务器下载的速度，我们可以配置并使用阿里云的Maven中央库镜像。对于Windows用户来说，配置方式如下：
------------------

### 1. 将%M2_HOME%/conf/settings.xml复制到%HOMEPATH%/.m2下

### 2. 修改settings.xml，在<mirrors>标签中加入如下标签：

```
		<mirror>
			<id>repository.central.aliyun</id>
			<name>Aliyun Mirror Repository</name>
			<mirrorOf>central</mirrorOf>
			<url>http://maven.aliyun.com/nexus/content/groups/public</url>
		</mirror>
```






