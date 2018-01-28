# glome
an Orb-Script compiler


Glome (codename Stack) is an Orb-Script compiler for generating Orb-Weaver bytecodes that can be run on any OrbLeaf's powered devices,
it uses LALR parser generated by bison and flex to process sourcecode token for user script
the scripting language influenced by ECMAScript (ECMA262), C and C# with some modification 
to enable collaboration between application package
it support several features such as 
 * context/object oriented programming
 * lambda expression
 * lazy expression
 * string preprocessor
 * dynamic object management
 
the purpose of Orb-Script to provide easy programming for any embedded device (similar with PHP idea)
accessing direct low-level are only available through native APIs (which is implemented using syscall mechanism)
runtime processing are done by Orb-Weaver virtual machine (OWvM), each variable are treated as dynamic object therefore
it's type cannot be known during compiler process, OWVM will trigger an exception and terminate execution
when type operation didn't match with a specified object

feel free to provide a new insight of how an Orb-Script should be
