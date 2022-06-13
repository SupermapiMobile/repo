# repo

#### Setting
###### Project build.gradle
```build.gradle
buildscript {
    ext.kotlin_version = "1.4.10"
    repositories {
        maven {
            url "https://raw.githubusercontent.com/SupermapiMobile/repo/main"
            //or url "https://repo.eqgis.cn"
        }
        google()
        jcenter()
    }
    dependencies {
        classpath 'com.android.tools.build:gradle:4.1.2'
        classpath "org.jetbrains.kotlin:kotlin-gradle-plugin:$kotlin_version"
    }
}

allprojects {
    repositories {

        google()
        jcenter()
        maven {
            url "https://raw.githubusercontent.com/SupermapiMobile/repo/main"
            //or url "https://repo.eqgis.cn"
        }
    }
}

```

###### Module build.gradle
```build.gradle
...
dependencies {
    //...
    implementation 'com.supermap:sceneform-sm:11.0.0'
}
...
```
