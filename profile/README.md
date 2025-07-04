Repository overview
-------------------

Devops: [e2immu-devops](https://github.com/e2immu/e2immu-devops).

Source code:

| main     | sub                                                             | subsub          | description                    |
|----------|-----------------------------------------------------------------|-----------------|--------------------------------|
| analyzer | [modification](https://github.com/e2immu/analyzer-modification) | common          | Common analyzer classes |
| analyzer | [modification](https://github.com/e2immu/analyzer-modification) | io              | Reading and writing AnalyzedPackage files |
| analyzer | [modification](https://github.com/e2immu/analyzer-modification) | prepwork        | First steps in modification analysis (hidden content, variable info) |
| analyzer | [modification](https://github.com/e2immu/analyzer-modification) | linkedvariables | Variable linking analysis, @Modified, @Independent |
| analyzer | [run](https://github.com/e2immu/analyzer-run)                   | config          | Configuration |
| analyzer | [run](https://github.com/e2immu/analyzer-run)                   | main            | command line options, main method  |
| analyzer | [run](https://github.com/e2immu/analyzer-run)                   | gradleplugin    | Gradle plugin |
| analyzer | [runmvn](https://github.com/e2immu/analyzer-runmvn)             | mvnplugin       | Maven plugin |
| analyzer | [aapi](https://github.com/e2immu/analyzer-aapi)                 | archive         | Annotated APIs for JDK and common libraries, and their AnalyzedPackage files |
| analyzer | [aapi](https://github.com/e2immu/analyzer-aapi)                 | parser          | Annotated API parser and writer  |
| language | [cst](https://github.com/e2immu/language-cst)                   | analysis        | Analysis property-value definitions |
| language | [cst](https://github.com/e2immu/language-cst)                   | api             | Primary interfaces of the Common Syntax Tree |
| language | [cst](https://github.com/e2immu/language-cst)                   | impl            | Primary implementation of the Common Syntax Tree |
| language | [cst](https://github.com/e2immu/language-cst)                   | io              | JSON I/O for CST analysis objects |
| language | [cst](https://github.com/e2immu/language-cst)                   | print           | Formatter for the CST |
| language | [inspection](https://github.com/e2immu/language-inspection)     | api             | Common API for language inspection/resolution/path management |
| language | [inspection](https://github.com/e2immu/language-inspection)     | parser          | Implementation of the parsing and resolution aspects of the API |
| language | [inspection](https://github.com/e2immu/language-inspection)     | resource        | Implementation of the resource/input/path aspects of the API |
| language | [inspection](https://github.com/e2immu/language-inspection)     | integration     | Integration of inspection system. |
| language | [java](https://github.com/e2immu/language-java)                 | bytecode        | Byte code inspection using ASM |
| language | [java](https://github.com/e2immu/language-java)                 | parser          | Source parsing using CongoCC |
| util     | [external](https://github.com/e2immu/util-external)             | support         | Annotations, support classes, and support for Annotated APIs. JDK 8 project! |
| util     | [internal](https://github.com/e2immu/util-internal)             | graph           | A graph library that uses _jgraph_ as a dependency. Support for linearization of dependency graphs. |
| util     | [internal](https://github.com/e2immu/util-internal)             | util            | Utility classes shared by multiple projects. |


Naming conventions
------------------

_main_ _sub_ _subsub_, where the combinations _sub-subsub_ must also be unique.

Github repositories: _main-sub_

Gradle projects inside a repository: e2immu-_sub_-_subsub_, test projects test*subsub*

Gradle project publishing IDs: org.e2immu._main_ : e2immu-_sub-subsub_ : version

Java packages: org.e2immu._main_._sub_._subsub_
