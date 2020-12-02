# Command Query Separation
Funções OU fazem algo OU respondem/checam algo.
**NO side effects**

```java
if (set("username", "uncleBob"))
```

```java
public boolean set(String attribute, String value)
```

v2:
```java
setAndCheckIfExists()
```

v3:
```java
if (attributeExists("username")) {
  setAttribute("username", "unclebob")
}
```