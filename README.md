# gradle plugin file

## 使用

> aar字符串加密插件, 全面支持`windows`、`mac`版本

1. 下载所需的依赖库

依赖库包括`baksmali-2.0.jar`、`smali-2.0.jar`、`dex2jar-2.0`、`smali_string_obfuscator`

2. 在library module下添加插件

```
apply from: 'https://andrsdk.github.io/gradle/pack.gradle'
```

3. 添加所需的运行参数

sdk的信息，用于最终生成的aar的名称和pom.xml里面的信息，在项目下的build.gradle下配置，如:

``` 
// sdk的名称
ext.sdk_name = 'function_blocksdk'
// sdk的版本号
ext.sdk_version = '2.0.0'
// sdk的依赖
ext.sdk_dependencies = []
```

在local.properties里面添加依赖库的目录

```
secret_home=D\:\\01_CODE\\secret
```

4. 运行

```
执行模块下的pack命令
```
