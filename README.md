# Live-Templates
分享个人 IntelliJ idea Live Template 配置,希望可以帮助大家提高编程效率,如果你那也有一些好用的template欢迎添加.

对于Live Template 还熟悉的童鞋可以先查看[**本文**](http://blog.xiaohansong.com/2017/03/17/idea-live-templates/).
## 实体类相关

Abbreviation : pi

Description : private Integer

Template text:
```
/**
 * $var1$
 */
private Integer $end$;

```
****
Abbreviation : pl

Description : private list

Template text:
```
/**
 * $var1$
 */
private List<$var2$> $end$;

```
****
Abbreviation : pm

Description : private map

Template text:
```
/**
 * $var1$
 */
private Map<$var2$, $var3$> $end$;

```
****
Abbreviation : ps

Description : private String

Template text:
```
/**
 * $var1$
 */
private String $end$;

```
****
Abbreviation : pss

Description : private Set

Template text:
```
/**
 * $var1$
 */
private Set<$var2$> $end$;

```
****
## 通用

Abbreviation : list

Description : list

作用域 : Java.Statement(其他的不用选)

Template text:
```
List<$var1$> list = new ArrayList<>();

```
****
Abbreviation : map

Description : map

作用域 : Java.Statement(其他的不用选)

Template text:
```
Map<$var1$, $var2$> map = new HashMap<>();

```
****

Abbreviation : set

Description : set

作用域 : Java.Statement(其他的不用选)

Template text:
```
Set<$var1$> set = new HashSet<>();

```

## log相关

Abbreviation : param

Description : log info method params

Variables : 

+ end = methodName()
+ params = groovyScript("'\"' + _1.collect { it + ' = [\" + ' + it + ' + \"]'}.join(', ') + '\"'", methodParameters())

Template text:
```
log.info("$end$ :" + $params$);

```
