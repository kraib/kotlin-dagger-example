kotlin-dagger-example
=====================

This project demonstrate how to setup an Android Project with Kotlin and Dagger 2.

It's based on Dagger 2 [example](https://github.com/google/dagger/tree/master/examples/android-simple)

##Known issues/limitations

1. Classes and interfaces that Dagger use for generating implementations must be kept in Java. If it's moved to Kotlin it won't be generated e.g. `AndroidModule`, `ApplicationComponent`

Thanks to `apt` library it's possible to use dagger injection in Kotlin.
There is also 'kapt' library from JetBrains but it requires using `SNAPSHOT` version of kotlin plugin.
After official release of `kapt` I will try to use it and see if dagger's classes can be moved to Kotlin.

##More than Dagger

This sample project includes some more dependencies which are very usefull. It's like a base setup for almost every project using Kotlin.
So you will find there Anko libraries. You can uncomment Anko's DSL libraries if you need them.
There is also a set of Rx dependencies. Rx works really great with Kotlin.
At last but not least there my favourite networking dependencies from Square.