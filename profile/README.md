Repository overview
-------------------

| main     | sub                                                             | subsub        | jdk | description                    |
|----------|-----------------------------------------------------------------|---------------|:--:|--------------------------------|
| analyzer | [shallow](https://github.com/e2immu/analyzer-shallow)           | aapi          | 8  | Annotated APIs for JDK and common libraries |
| analyzer | [shallow](https://github.com/e2immu/analyzer-shallow)           | analyzer      | 17 | Annotated API reader and shallow analyzer  |
| analyzer | [modification](https://github.com/e2immu/analyzer-modification) | gradleplugin  | 17 | Gradle plugin |
| analyzer | [modification](https://github.com/e2immu/analyzer-modification) | hiddencontent | 17 | First step in modification analysis |
| analyzer | [modification](https://github.com/e2immu/analyzer-modification) | immutable     | 17 | Determine @Container, @Immutable |
| analyzer | [modification](https://github.com/e2immu/analyzer-modification) | integration   | 17 | Entry point for modification analyzer usage |
| analyzer | [modification](https://github.com/e2immu/analyzer-modification) | linking       | 17 | Variable linking analysis, @Modified, @Independent |
| analyzer | [modification](https://github.com/e2immu/analyzer-modification) | variableinfo  | 17 | Build VariableInfo objects |
| language | [cst](https://github.com/e2immu/language-cst)                   | api           | 17 | Primary interfaces of the Common Syntax Tree |
| language | [cst](https://github.com/e2immu/language-cst)                   | impl          | 17 | Primary implementation of the Common Syntax Tree |
| language | [cst](https://github.com/e2immu/language-cst)                   | io            | 17 | JSON I/O for CST analysis objects |
| language | [cst](https://github.com/e2immu/language-cst)                   | print         | 17 | Formatter for the CST |
| language | [inspection](https://github.com/e2immu/language-inspection)     | api           | 17 | Common API for language inspection/resolution/path management |
| language | [inspection](https://github.com/e2immu/language-inspection)     | parser        | 17 | Implementation of the parsing and resolution aspects of the API |
| language | [inspection](https://github.com/e2immu/language-inspection)     | resource      | 17 | Implementation of the resource/input/path aspects of the API |
| language | [java](https://github.com/e2immu/language-java)                 | bytecode      | 17 | Byte code inspection using ASM |
| language | [java](https://github.com/e2immu/language-java)                 | parser        | 17 | Source parsing using CongoCC |
| util     | [external](https://github.com/e2immu/util-external)             | support       | 8  | Annotations, support classes, and support for Annotated APIs |
| util     | [internal](https://github.com/e2immu/util-internal)             | graph         | 17 | A graph library that uses _jgraph_ as a dependency. Support for linearization of dependency graphs. |
| util     | [internal](https://github.com/e2immu/util-internal)             | util          | 17 | Utility classes shared by multiple projects. |


Naming conventions
------------------

_main_ _sub_ _subsub_, where the combinations _sub-subsub_ must also be unique.

Github repositories: _main-sub_

Gradle projects inside a repository: e2immu-_sub_-_subsub_, test projects test*subsub*

Gradle project publishing IDs: org.e2immu._main_ : e2immu-_sub-subsub_ : version

Java packages: org.e2immu._main_._sub_._subsub_
