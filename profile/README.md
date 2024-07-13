Repository overview
-------------------

| main     | sub                                                             | subsub        | description                    |
|----------|-----------------------------------------------------------------|---------------|--------------------------------|
| analyzer | [modification](https://github.com/e2immu/analyzer-modification) | hiddencontent | First step in modification analysis |
| analyzer | [modification](https://github.com/e2immu/analyzer-modification) | immutable     | Determine @Container, @Immutable |
| analyzer | [modification](https://github.com/e2immu/analyzer-modification) | integration   | Entry point for modification analyzer usage |
| analyzer | [modification](https://github.com/e2immu/analyzer-modification) | linking       | Variable linking analysis, @Modified, @Independent |
| analyzer | [modification](https://github.com/e2immu/analyzer-modification) | variableinfo  | Build VariableInfo objects |
| analyzer | [run](https://github.com/e2immu/analyzer-run)                   | config        | Configuration |
| analyzer | [run](https://github.com/e2immu/analyzer-run)                   | main          | command line options, main method  |
| analyzer | [run](https://github.com/e2immu/analyzer-run)                   | gradleplugin  | Gradle plugin |
| analyzer | [shallow](https://github.com/e2immu/analyzer-shallow)           | aapi          | Annotated APIs for JDK and common libraries. |
| analyzer | [shallow](https://github.com/e2immu/analyzer-shallow)           | analyzer      | Annotated API reader and shallow analyzer  |
| language | [cst](https://github.com/e2immu/language-cst)                   | api           | Primary interfaces of the Common Syntax Tree |
| language | [cst](https://github.com/e2immu/language-cst)                   | impl          | Primary implementation of the Common Syntax Tree |
| language | [cst](https://github.com/e2immu/language-cst)                   | io            | JSON I/O for CST analysis objects |
| language | [cst](https://github.com/e2immu/language-cst)                   | print         | Formatter for the CST |
| language | [inspection](https://github.com/e2immu/language-inspection)     | api           | Common API for language inspection/resolution/path management |
| language | [inspection](https://github.com/e2immu/language-inspection)     | parser        | Implementation of the parsing and resolution aspects of the API |
| language | [inspection](https://github.com/e2immu/language-inspection)     | resource      | Implementation of the resource/input/path aspects of the API |
| language | [inspection](https://github.com/e2immu/language-inspection)     | integration   | Integration of inspection system. |
| language | [java](https://github.com/e2immu/language-java)                 | bytecode      | Byte code inspection using ASM |
| language | [java](https://github.com/e2immu/language-java)                 | parser        | Source parsing using CongoCC |
| util     | [external](https://github.com/e2immu/util-external)             | support       | Annotations, support classes, and support for Annotated APIs. JDK 8 project! |
| util     | [internal](https://github.com/e2immu/util-internal)             | graph         | A graph library that uses _jgraph_ as a dependency. Support for linearization of dependency graphs. |
| util     | [internal](https://github.com/e2immu/util-internal)             | util          | Utility classes shared by multiple projects. |


Naming conventions
------------------

_main_ _sub_ _subsub_, where the combinations _sub-subsub_ must also be unique.

Github repositories: _main-sub_

Gradle projects inside a repository: e2immu-_sub_-_subsub_, test projects test*subsub*

Gradle project publishing IDs: org.e2immu._main_ : e2immu-_sub-subsub_ : version

Java packages: org.e2immu._main_._sub_._subsub_
