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
    val a: Int = 1  // immediate assignment
    val b = 2   // `Int` type is inferred
    val c: Int  // Type required when no initializer is provided
    c = 3       // deferred assignment
    println("a = $a, b = $b, c = $c")
}
```

#### Conditional expressions
```kotlin
1. In Kotlin, if is an expression, i.e. it returns a value. Therefore there is no ternary operator (condition ? then : else), because ordinary if works fine in this.

EXAMPLE 1:-

fun maxOf(a: Int, b: Int) = if (a > b) a else b
fun main() {
    println("max of 0 and 42 is ${maxOf(0, 42)}")
}
OUTPUT
max of 0 and 42 is 42
```
```kotlin
EXAMPLE 2:-
Nullable values and null checks:-

fun parseInt(str: String):Int?{
    return str.toIntOrNull()
}
fun printProduct(arg1:String,arg2:String){
    val x = parseInt(arg1)
    val y = parseInt(arg2)
    
    if(x == null){
        println("wrong number format in arg1:'$arg1'")
        return
    }
    if(y == null){
        println("wrong number format in arg2:'$arg2'")
        return
    }
    println(x * y)
}
fun main() {
    printProduct("6","7")
    printProduct("a","7")
    printProduct("99","b")
}
OUTPUT

42
wrong number format in arg1:'a'
wrong number format in arg2:'b'
```


