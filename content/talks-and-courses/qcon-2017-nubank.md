# nuBank: Architecturing a modern financial institution

#Kafka #Clojure #QCon talk

https://www.youtube.com/watch?v=VYuToviSx5Q

2017

- [ ] Add screenshotted notes from `talk-nubank`

- Opinion:liked

---

## Notes

- NOTE TO SELF: Always assume there's a standard or convention somewhere

- The ISO document is not public(?)
.. information is missing anyways, and needs to be filled from VISA or Mastercard

- They use Datomic transaction identifiers (or whatever they're called) to ensure messages are idempotent and then use it as a correlation id to not re process the same thing more than once. Not replying on Kafka's features.

- Correlation id is a concept(?)

---

END.
