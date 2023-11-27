# responsive-layout-grid-compose
compose용 responsive layout grid 입니다. 
_성능 개선 및 오류에 관련한 모든 피드백을 언제나 환영합니다.😊_
<br>
<br>
# Material Guideline
[Google Material Guideline](https://m2.material.io/design/layout/responsive-layout-grid.html)을 따릅니다.
<br>
>        * Row Break Point
>         _ResponsiveRow에서 totalColumns이 AUTO 일 때 자동으로 지정됩니다.(gutter는 공식 가이드라인이 제공되지 않으므로 config에서 별도 지정 가능합니다.)_
>         Type | Screen Size | Margin | Body | Layout columns | Gutter Default
>         `Phone` Extra-small | 0-599 | 16dp | Scaling | 4 | 16dp
>         'Tablet Small` Small | 600-904 | 32dp | Scaling | 8 | 24dp
>         `Tablet Large` Small | 905-1239 | Scaling | 840dp | 12 | 24dp
>         `Laptop` Medium | 1240-1439 | 200dp | Scaling | 12 | 32dp
>         `Desktop` Large | 1440+ | Scaling | 1040dp | 12 | 32dp
<br>
<br>
# Set up for use
현재 [최신버전](https://jitpack.io/#nyangzzi/responsive-layout-grid-compose)은 `-` 입니다.
<br>
1. Add the JitPack repository to your build file (settings.gradle)
>	* groovy
>	```groovy
>	dependencyResolutionManagement {
>		repositoriesMode.set(RepositoriesMode.FAIL_ON_PROJECT_REPOS)
>		repositories {
>			mavenCentral()
>			maven { url 'https://jitpack.io' }
>		}
>	}
>	```
>
>	* kotlin
>	```kotlin
>	dependencyResolutionManagement {
>		repositoriesMode.set(RepositoriesMode.FAIL_ON_PROJECT_REPOS)
>		repositories {
>			mavenCentral()
>			maven { url = uri("https://www.jitpack.io" ) }
>		}
>	}
>	```
<br>
2. Add the dependency 
> Tag에 적용할 버전을 입력합니다.
>	* groovy
>	```groovy
>	dependencies {
>	        implementation 'com.github.nyangzzi:responsive-layout-grid-compose:Tag'
>	}
>	```
>
>	* kotlin
>	```kotlin
>	dependencies {
>	        implementation("com.github.nyangzzi:responsive-layout-grid-compose:Tag")
>	}
>	```
<br>
<br>
# How to use
Row와 Column 2가지 버전을 제공합니다.
(업데이트 예정입니다.)
<br>
<br>
# Dependencies
* 
<br>
<br>
# File Structure
```
Core
│  ResponsiveConfig.kt
│  Util.kt
│  
├─column
│      ResponsiveColumn.kt
│      ResponsiveColumnScope.kt
│      
└─row
       ResponsiveRow.kt
       ResponsiveRowScope.kt
       RowBreakPoint.kt
```

