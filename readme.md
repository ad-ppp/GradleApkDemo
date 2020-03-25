# gradle  研究

1. 理解Gradle构建的生命周期
2. 展示如何调用子module的 task
3. 构建差异化 apk
4. Hook点, Gradle提供了非常多的钩子供开发人员修改构建过程中的行为
5. 动态改变Task依赖关系
6. [动态修改label示例](https://stackoverflow.com/questions/32092665/resolve-application-label-for-each-build-type)
7. [Versioning your builds via "version.properties" file](https://riptutorial.com/android/example/7837/versioning-your-builds-via--version-properties--file)


### 实用记录

1. `gradle --help`
2. 查看task依赖关系： gradle.plugin.com.dorongold.plugins:task-tree:1.3.1
gradle ${taskName} tasktree --no-repeat 比如`gradle :app:assembleVariant_aDebug tasktree --no-repeat`
3. 部分配置可以参考 telegram.gradle

### 构建差异化 apk 遇到问题记录

1. [All flavors must now belong to a named flavor dimension](https://developer.android.com/studio/build/build-variants?utm_source=android-studio#product-flavors)

### Thanks to
1. [Gradle基础 - 构建生命周期和Hook技术](https://www.jianshu.com/p/0acdb31eef2d)
2. [构建差异化 apk-Gradle妙用，统一化自动依赖管理](https://mp.weixin.qq.com/s/Lhae-ou5gEcXjUFnuVCwaw)
3. [Android Gradle Plugin源码分析](https://www.jianshu.com/p/11f030b2034f)