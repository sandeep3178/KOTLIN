# KOTLIN
```
Kotlin provides the ability to target JavaScript. It does so by transpiling Kotlin to JavaScript. The current implementation targets ECMAScript 5.1 but there are plans to eventually target ECMAScript 2015 as well.

```
## Program entry point
```kotlin
fun sum(a: Int, b: Int) = a + b
fun main() {
    println("sum of 19 and 23 is ${sum(19, 23)}")
}
```
### Variables
``` kotlin
fun main() {
    val a: Int = 1  
    val b = 2   
    val c: Int  
    c = 3       
    println("a = $a, b = $b, c = $c")
}
```

#### Conditional expressions
```kotlin
In Kotlin, if is an expression, i.e. it returns a value. Therefore there is no ternary operator (condition ? then : else), because ordinary if works fine in this.

EXAMPLE:-

fun maxOf(a: Int, b: Int) = if (a > b) a else b
fun main() {
    println("max of 0 and 42 is ${maxOf(0, 42)}")
}
```

