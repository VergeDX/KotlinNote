# Basic Syntax
Reference:  
[https://www.kotlincn.net/docs/reference/basic-syntax.html](https://www.kotlincn.net/docs/reference/basic-syntax.html)  
[https://kotlinlang.org/docs/reference/basic-syntax.html](https://kotlinlang.org/docs/reference/basic-syntax.html)

Package definition and imports:  
IDEA can also offer help.

Program entry point:  
main function can also accept args:  
[https://www.programiz.com/kotlin-programming/hello-world](https://www.programiz.com/kotlin-programming/hello-world)
`````kotlin
fun main(args : Array<String>) {
    println("Hello, World!")
}
`````

Functions:  
Kotlin `Unit` just like Java `void`, but in Kotlin;  
`Unit` return type can be omitted.

If a variable can be `null`, must marked as nullable `?`
`````kotlin
fun parseInt(str: String): Int? {
    // ...
}
`````

# Idioms
Creating DTOs (POJOs/POCOs):
`````kotlin
data class Customer(val name: String, val email: String)
`````

provides a Customer class with the following functionality:  
`getter()` & `setter() [only for var]`  
`equals()`, `hashCode()`, `toString() [Customer(name=VergeDX, email=wxy20001225@126.com)]`  
`copy() [copy a new instance and modify it's property]`  
`component1()` `component2()` etc. They are using in `Destructuring Declarations`.

Using ranges:  
`..`, `until`, `step`, `downTo`
`````kotlin
// Empty range! using downTo instead.
for (x in 10..1) {}
`````
