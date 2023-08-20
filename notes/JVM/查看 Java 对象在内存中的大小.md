# 查看 Java 对象在内存中的大小

**方法一：使用 lucene-core**

```xml
  <dependency>
      <groupId>org.apache.lucene</groupId>
      <artifactId>lucene-core</artifactId>
      <version>4.0.0</version>
  </dependency>
```

```java
Object obj = new Object();
System.out.println(RamUsageEstimator.sizeOf(obj));
System.out.println(RamUsageEstimator.humanSizeOf(obj));
```

**方法二：JDK 自带方法 ObjectSizeCalculator**

```java
Object obj = new Object();
System.out.println(ObjectSizeCalculator.getObjectSize(obj));
```

