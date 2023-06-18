# GlueGen, Native Binding Generator for Java™

[Original document location](https://jogamp.org/cgit/gluegen.git/about/)

## Git Repository
This project's canonical repositories is hosted on [JogAmp](https://jogamp.org/cgit/gluegen.git/).

## Overview
[GlueGen](https://jogamp.org/gluegen/www/) is a compiler for function and data-structure declarations, 
generating Java™ and JNI C code offline at compile time 
and allows using native libraries within your Java™ application.

It reads ANSI C header files
and separate configuration files which provide control over many
aspects of the glue code generation. GlueGen uses a complete ANSI C
parser and an internal representation (IR) capable of representing all
C types to represent the APIs for which it generates interfaces. It
has the ability to perform significant transformations on the IR
before glue code emission. 

GlueGen can produce native foreign function bindings to Java™ as well as
map native data structures to be fully accessible from Java™ including 
potential calls to embedded function pointer.

GlueGen is also capable to bind even low-level APIs such as the Java™ Native Interface (JNI) and
the AWT Native Interface (JAWT) back up to the Java™ programming language.

GlueGen utilizes [JCPP](https://jogamp.org/cgit/jcpp.git/about/), migrated C preprocessor written in Java™.

GlueGen is used for the [JogAmp](https://jogamp.org) projects
[JOAL](https://jogamp.org/cgit/joal.git/about/),
[JOGL](https://jogamp.org/cgit/jogl.git/about/) and
[JOCL](https://jogamp.org/cgit/jocl.git/).

GlueGen is part of [the JogAmp project](https://jogamp.org).

**The JogAmp project needs funding and we offer [commercial support](https://jogamp.org/wiki/index.php?title=Maintainer_and_Contacts#Commercial_Support)!**<br/>
Please contact [Göthel Software (Jausoft)](https://jausoft.com/).

### License
See [LICENSE.txt](LICENSE.txt).

## Documentation

* [GlueGen Java™ API-Doc](https://jogamp.org/deployment/jogamp-next/javadoc/gluegen/javadoc/)
* [GlueGen Native Data & Function Mapping for Java™](doc/GlueGen_Mapping.md)
* [GlueGen Manual](doc/manual/)
* [JogAmp's MacOS Version Support](doc/JogAmpMacOSVersions.md)
* [How To Build](https://jogamp.org/gluegen/doc/HowToBuild.html)

## Build Requirements
Check [GlueGen's HowToBuild](https://jogamp.org/gluegen/doc/HowToBuild.html).

## Directory Organization:
```
make/           Build-related files and the main build.xml
doc/            Documentation
jcpp/           JCPP (git sub-module), migrated C preprocessor written in Java
src/            The actual source for the JOAL APIs.
src/junit/      Unit tests
test/           Standalone manual tests
build/          (generated directory) Where the Jar and DLL files get built to
www/            JOAL project webpage files
```

## Contact Us
- JogAmp             [http://jogamp.org/](https://jogamp.org/)
- JOAL Web           [http://jogamp.org/](https://jogamp.org/joal/)
- Forum/Mailinglist  [http://forum.jogamp.org/](https://forum.jogamp.org/)
- Repository         [http://jogamp.org/git/](https://jogamp.org/git/)
- Wiki               [https://jogamp.org/wiki/](https://jogamp.org/wiki/)
- Maintainer         [https://jogamp.org/wiki/index.php/Maintainer_and_Contacts](https://jogamp.org/wiki/index.php/Maintainer_and_Contacts)
- Sven's Blog        [https://jausoft.com/blog/tag/jogamp/](https://jausoft.com/blog/tag/jogamp/)
- Email              sgothel _at_ jausoft _dot_ com

## History
Since roughly 2010, GlueGen development has been continued
by individuals of the JogAmp community, see git log for details.
