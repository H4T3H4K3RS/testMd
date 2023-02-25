

# <?>
The `<?>` is a shorthand for `<? extends Object>`. It means that the type parameter can be any type.

**Example**
```java
public class GenericClass<T> {
  private T obj;
  public GenericClass(T obj) {
    this.obj = obj;
  }
}
GenericClass<?> gc = new GenericClass<String>("Hello");
//Here, gc can refer to a GenericClass of any type, since we used the ? wildcard.
```

# <? extends T>
The `<? extends T>` wildcard means that the type parameter is either the type T or a subtype of T. This is known as an upper bounded wildcard.

**Example**
```java
public class GenericClass<T> {
  private T obj;
  public GenericClass(T obj) {
    this.obj = obj;
  }
}
GenericClass<? extends Number> gc = new GenericClass<Integer>(1);
//Here, gc can refer to a GenericClass of type Integer, Double, Float, etc., since Integer is a subtype of Number.
```

# <? super T>
The `<? super T>` wildcard means that the type parameter is either the type T or a super type of T. This is known as a lower bounded wildcard.

**Example**
```java
public class GenericClass<T> {
  private T obj;
  public GenericClass(T obj) {
    this.obj = obj;
  }
}
GenericClass<? super Integer> gc = new GenericClass<Number>(1.0);
//Here, gc can refer to a GenericClass of type Integer, Number, Object, etc., since Number is a supertype of Integer.
```