# About Java Versioning

For #ReMonke: The Fantastic Flip of a monkey

---

Skimmed #liked
https://csis.pace.edu/~bergin/dcs/versioning/index.html

---

Read #done #liked http://wiki.c2.com/?JavaVersioning

---

Read done #meh
Anti #pattern?
For Java RMI Versioning
Za3ma to add version identifiers to exported interfaces (semver)

---

## Constant interface
https://en.wikipedia.org/wiki/Constant_interface#%3A%7E%3Atext%3DIn_the_Java_programming_language%2Csyntactic_access_to_those_constants.?wprov=sfla1

---

#DesignPattern, as in #Java's Serializable used before Java 1.5 had annotations.

Marker interface pattern
https://en.wikipedia.org/wiki/Marker_interface_pattern?wprov=sfla1

---

TLDR: Why not if the constants represent a concept/value that is respected by the contact.
Real examples are libraries such some awt interfaces.

KAITO: the keyword here is "concept", as in semver VERSION

https://softwareengineering.stackexchange.com/questions/49572/is-it-a-bad-practice-to-have-an-interface-to-define-constants

---

Mentioned the Constant Interface pattern.
Mentioned a Constants and Utils class. Constants is a good name tbh.
Warned against this scenario: You compile a specific class, the Java compiler inlines the constant value in the generated .class file, you change the constant value's declaration and compile other classes. Now you get inconsistent constant values.

Constants in Java
https://www.baeldung.com/java-constants-good-practices

---

Yes, it worked for him but he needed a "middleman" to register classes locally.

https://community.oracle.com/tech/developers/discussion/2160300/running-one-rmiregistry-for-multiple-remote-object-servers

---

`FindVersion(semver)`
`FindAllVersions(semver)`

Using `Registry::list`
* [Registry (Java Platform SE 8)](https://docs.oracle.com/javase/8/docs/api/java/rmi/registry/Registry.html#list--)


Export to RMI: getSemVersion() + getHashCode()
then use to sort and compare:
https://github.com/vdurmont/semver4j
