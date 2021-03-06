Wire Gradle Plugin
==================

A Gradle plugin for generating Java code for your protocol buffer definitions with Wire

How to use
----------

in $projectRoot/build.gradle

```
repositories {
    jcenter()
}
```
```    
dependencies {
    classpath 'com.jiechic.library.wire:wire-gradle-plugin:1.0.2'
}
```

in module/build.gradle
```
apply plugin: 'com.squareup.wire'

dependencies {
    compile 'com.squareup.wire:wire-runtime:2.2.0'
}
```



Configure
---------

delault proto srcDirs
```
src/main/proto
```

custom proto srcDirs

```
sourceSets {
    main {
        wire {
            srcDirs += "proto/src"
        }
    }
}
```

wire{
    android = false
}


License
-------

    Copyright 2015 Square, Inc.

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
