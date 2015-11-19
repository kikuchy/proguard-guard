# ProGard-Guard :closed_lock_with_key:

*WIP*


## Concept

[ProGuard](http://developer.android.com/intl/tools/help/proguard.html) is useful to guard our products.
But we often forget settings of ProGuard.
(cf. `proguard-confg.txt`, `proguard-rules.pro` or etc...)

*ProGuard-Guard* will be release us from ProGuard setting files.

Anotate your classes and compile it.
ProGuard setting files are generated automatically!


## Usage

### 1. Add ProGuard setting (Only first once!)

```
# Relative path is OK.
@(your_project_root)/build/proguard-rules-gen.pro
```



### 2. Annotate your codes

```java
// Annotate class with @Keep is the same proguard's "-keep" option.

@Keep
@DonwWarn
public class AweSomeExecutor$$AutoGenerated {

    ...

}
```


### 3. Compile your codes

That's all!
Happy coding!!