# Weakrefs

[Weak reference | Wikipedia](https://en.wikipedia.org/wiki/Weak_reference)


## JavaScript

- WeakRefs TC39 proposal: https://github.com/tc39/proposal-weakrefs
    * "WeakRef and FinalizationRegistry are now Stage 4, since the July 2020 TC39 meeting"

- Spec: [WeakRefs proposal | TC39.ES](https://tc39.es/proposal-weakrefs/)

- [WeakRef - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/WeakRef)


## Java

### WeakReference
https://docs.oracle.com/javase/8/docs/api/java/lang/ref/WeakReference.html
    * "Since 1.2"

### WeakHashMap
[WeakHashMap (Java Platform SE 8 )](https://docs.oracle.com/javase/8/docs/api/java/util/WeakHashMap.html)

### Weak Hash Set using `Collections::newSetFromMap`
- [Collections::newSetFromMap (Java Platform SE 8 )](https://docs.oracle.com/javase/8/docs/api/java/util/Collections.html#newSetFromMap-java.util.Map-)

`public static <E> Set<E> newSetFromMap(Map<E,Boolean> map)`  
Returns a set backed by the specified map. The resulting set displays the same ordering, concurrency, and performance characteristics as the backing map. In essence, this factory method provides a [`Set`](https://docs.oracle.com/javase/8/docs/api/java/util/Set.html "interface in java.util") implementation corresponding to any [`Map`](https://docs.oracle.com/javase/8/docs/api/java/util/Map.html "interface in java.util") implementation. There is no need to use this method on a [`Map`](https://docs.oracle.com/javase/8/docs/api/java/util/Map.html "interface in java.util") implementation that already has a corresponding [`Set`](https://docs.oracle.com/javase/8/docs/api/java/util/Set.html "interface in java.util") implementation (such as [`HashMap`](https://docs.oracle.com/javase/8/docs/api/java/util/HashMap.html "class in java.util") or [`TreeMap`](https://docs.oracle.com/javase/8/docs/api/java/util/TreeMap.html "class in java.util")).

```java
Set<Object> weakHashSet = Collections.newSetFromMap(
    new WeakHashMap<Object, Boolean>());
```


## CSharp

- [WeakReference Class (System) | Microsoft Docs](https://docs.microsoft.com/en-us/dotnet/api/system.weakreference?view=netframework-4.8)

- [ConditionalWeakTable<TKey,TValue> Class (System.Runtime.CompilerServices) | Microsoft Docs](https://docs.microsoft.com/en-us/dotnet/api/system.runtime.compilerservices.conditionalweaktable-2?view=netframework-4.8)

---

END.
