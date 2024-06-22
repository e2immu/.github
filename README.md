Repository overview
-------------------

| main     | sub                                                            | subsub          | jdk | description                    |
|----------|----------------------------------------------------------------|-----------------|:---:|--------------------------------|
| analyzer | shallow  | aapi | 17 | Annotated API parsing |
| analyzer | shallow  | minimal | 17 | Minimal analyzer   |
| analyzer | shallow  | integration | 17 | Entry point for shallow analyzer usage |
| analyzer | modification | hiddencontent | 17 | First step in modification analysis |
| analyzer | modification | immutable     | 17 | Determine @Container, @Immutable |
| analyzer | modification | integration   | 17 | Entry point for modification analyzer usage |
| analyzer | modification | linking       | 17 | Variable linking analysis, @Modified, @Independent |
| analyzer | modification | variableinfo  | 17 | Build VariableInfo objects |
| language | [cst](https://github.com/e2immu/language-cst)                 | api        | 17  | Primary interfaces of the Common Syntax Tree |
| language | [cst](https://github.com/e2immu/language-cst)                 | impl       | 17  | Primary implementation of the Common Syntax Tree |
| language | [cst](https://github.com/e2immu/language-cst)                 | io         | 17  | JSON I/O for CST analysis objects |
| language | [cst](https://github.com/e2immu/language-cst)                 | print      | 17  | Formatter for the CST |
| language | [inspection](https://github.com/e2immu/language-inspection)   | api        | 17  | Common API for language inspection/resolution/path management |
| language | [inspection](https://github.com/e2immu/language-inspection)   | parser     | 17  | Implementation of the parsing and resolution aspects of the API |
| util     | [external](https://github.com/e2immu/util-external)           | support    | 8 | Annotations, support classes, and support for Annotated APIs |
| util     | [internal](https://github.com/e2immu/util-internal)           | graph      | 17 | A graph library that uses _jgraph_ as a dependency. Support for linearization of dependency graphs. |


Naming conventions
------------------

_main_ _sub_ _subsub_, where the combinations _sub-subsub_ must also be unique.

Github repositories: _main-sub_

Gradle projects inside a repository: e2immu-_sub_-_subsub_, test projects test*subsub*

Gradle project publishing IDs: org.e2immu._main_ : e2immu-_sub-subsub_ : version

Java packages: org.e2immu._main_._sub_._subsub_
