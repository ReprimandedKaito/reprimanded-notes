# JSONPath
#json

- Supported by Apache Camel.
    * [JSONPath :: Apache Camel](https://camel.apache.org/components/3.17.x/languages/jsonpath-language.html)
    * Camel references [json-path/JsonPath | GitHub](https://github.com/json-path/JsonPath) -- a Java JsonPath implementation.

```java
// Source:
// https://camel.apache.org/components/3.17.x/languages/jsonpath-language.html#_examples

from("queue:books.new")
  .choice()
    .when().jsonpath("$.store.book[?(@.price < 10)]")
      .to("jms:queue:book.cheap")
    .when().jsonpath("$.store.book[?(@.price < 30)]")
      .to("jms:queue:book.average")
    .otherwise()
      .to("jms:queue:book.expensive");
```

---

- Does `jq` (https://stedolan.github.io/jq) use or support JSONPath?
No, but they are similar in some aspects. See: [For JSONPath users · stedolan/jq Wiki · GitHub](https://github.com/stedolan/jq/wiki/For-JSONPath-users) (visited 2022-07-02).

- jq mentioned **JSON Pointer**:
    * https://datatracker.ietf.org/doc/html/rfc6901 JavaScript Object Notation (JSON) Pointer
    * https://www.baeldung.com/json-pointer Overview of JSON Pointer | Baeldung
        + [ ] Test.
    * https://jcp.org/en/jsr/detail?id=374 JSR 374: JavaTM API for JSON Processing 1.1
        + [ ] Download javadoc

---

END.
