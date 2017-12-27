

# anyRTC娃娃机客户端信令安卓SDK






>方式一（推荐）（正在审核中！即将生效）

添加Jcenter仓库 Gradle依赖：

```
dependencies {
    compile 'org.anyrtc:anyrtcwawaclient:1.0.0'
}
```

或者 Maven
```
<dependency>
  <groupId>org.anyrtc</groupId>
  <artifactId>anyrtcwawaclient</artifactId>
  <version>1.0.0</version>
  <type>pom</type>
</dependency>
```

>方式二



>1. 将下载DEMO中的anyrtcwawaclient-release.aar文件放入项目的libs目录中
>2. 在Model下的build.gradle文件添加如下代码依赖anyRTCWaWaClient SDK

```
android
{

 repositories {
        flatDir {dirs 'libs'}
    }
    
 }
    
```
```
dependencies {
    compile(name: 'anyrtcwawaclient-release', ext: 'aar')
    //还需添加第三方socket框架
    compile('io.socket:socket.io-client:1.0.0') {
        exclude group: 'org.json', module: 'json'
    }
}
```
