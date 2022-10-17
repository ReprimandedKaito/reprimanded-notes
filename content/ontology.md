# Ontology

Kaito's questions:
- Again, what is an ontology?
- What are the differences between an ontology and a (well-designed/generic) data model?
- What are the differences between an ontology and a (well-designed/generic) database?
- Is an ontological database an ontology?

## Tools

- Protégé

- WebProtégé
    * [ ] READ:
        WebProtégé: A Cloud-Based Ontology Editor
        https://arxiv.org/ftp/arxiv/papers/1902/1902.08251.pdf
    * [ ] TRY?

- [ ] VOWL
    * [ ] WebVOWL http://www.visualdataweb.de/webvowl/
    * [ ] LD-VOWL http://vowl.visualdataweb.org/ldvowl/

## Reading list

### Notes: "Data Modelling versus Ontology Engineering"

**TLDR**:
- [ ] _TBD_

- [ ] READ

`\cite{spyns2002data}`
[`[researchgate:publication:220416072]`](https://www.researchgate.net/publication/220416072)
`[saved:spyns2002data.pdf]`

```bibtex notes-library.bibtex +=
@article{spyns2002data,
    author = {Spyns, Peter and Meersman, Robert and Jarrar, Mustafa},
    year = {2002},
    month = {03},
    pages = {12-17},
    title = {Data Modelling versus Ontology Engineering.},
    volume = {31},
    journal = {ACM SIGMOD Record},
    doi = {10.1145/637411.637413}
}
```


### Notes: "Ontology and database schema: What's the difference?"

**TLDR**
- [ ] _TBD_

[Ontology and database schema: What’s the difference? | edi-info.ir](http://www.dl.edi-info.ir/Ontology%20and%20database%20schema,%20What%20is%20the%20difference.pdf)

`[saved:uschold2015ontology.pdf]`


```bibtex
@article{uschold2015ontology,
  title={Ontology and database schema: What’s the difference?},
  author={Uschold, Michael},
  journal={Applied Ontology},
  volume={10},
  number={3-4},
  pages={243--258},
  year={2015},
  publisher={IOS Press}
}
```

---

### Notes: "Learning the differences between ontologies and conceptual schemas through ontology-driven information systems"

**TLDR**
- [ ] _TBD_

[Learning the differences between ontologies and conceptual schemas through ontology-driven information systems | PSU.edu](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.611.6908&rep=rep1&type=pdf)

`[saved:fonseca2007learning.pdf]`

```bibtex
@article{fonseca2007learning,
  title={Learning the differences between ontologies and conceptual schemas through ontology-driven information systems.},
  author={Fonseca, Frederico and Martin, James},
  journal={Journal of the Association for Information Systems},
  volume={8},
  number={2},
  pages={4},
  year={2007}
}
```

---

## Notes: "Ontology Development 101: A Guide to Creating Your First Ontology"

[Ontology Development 101: A Guide to Creating Your First Ontology | Protege.Stanford.edu](https://protege.stanford.edu/publications/ontology_development/ontology101-noy-mcguinness.html)

\cite{noy2001ontology}

**TLDR**:
It basically shows you how to create a "class diagram".
If you know UML and POO's best practices then you already know 80% of what that article teaches.


> Separating the domain knowledge from the operational knowledge is another common use of ontologies. We can describe a task of configuring a product from its components according to a required specification and implement a program that does this configuration independent of the products and components themselves (McGuinness and Wright 1998). We can then develop an ontology of PC-components and characteristics and apply the algorithm to configure made-to-order PCs. We can also use the same algorithm to configure elevators if we “feed” an elevator component ontology to it (Rothenfluh et al. 1996).
>
> -- "Why develop an ontology?" section

> Synonyms are just different names for a concept or a term. Therefore, we should not have a class called Shrimp and a class called Prawn, and, possibly a class called Crevette. Rather, there is one class, named either Shrimp or Prawn. Many systems allow associating a list of synonyms,  translations, or presentation names with a class. If a system does not allow this associations, synonyms could always be listed in the class documentation.
>
> -- "Ensuring that the class hierarchy is correct" section

> Most knowledge-representation systems allow multiple inheritance in the class hierarchy: a class can be a subclass of several classes. Suppose we would like to create a separate class of dessert wines, the Dessert wine class. The Port wine is both a red wine and a dessert wine.[4] Therefore, we define a class Port to have two superclasses: Red wine and Dessert wine. All instances of the Port class will be instances of both the Red wine class and the Dessert wine class. The Port class will inherit its slots and their facets from both its parents. Thus, it will inherit the value SWEET for the slot Sugar from the Dessert wine class and the tannin level slot and the value for its color slot from the Red wine class.
>
> -- "Multiple inheritance" section

```bibtex notes-library.bibtex +=
@misc{noy2001ontology,
    title = {Ontology development 101: A guide to creating your first ontology},
    author = {Noy, Natalya F and McGuinness, Deborah L and others},
    year = {2001},
    publisher = {Stanford knowledge systems laboratory technical report KSL-01-05 and~…}
    howpublished = "\url{https://protege.stanford.edu/publications/ontology_development/ontology101.pdf}"
}
```

---

## Notes: "Ontologies versus relational databases: Are they so different? A comparison"

**TLDR**:
I'm still (if not _more_) confused, lol.

> ## 4. Ontologies and DB communication
> 
> ### 4.1 Using the same conceptual modeling technique
> This proposal establishes that if an ontology and a database share the same conceptual representation, the data communication is easier.
> This is the Brockmans et al. (2006) approach that uses the same UML representation for generating both an ontology schema and a database schema.
> Consequently, this proposal requires the use of specific tools and representation mechanisms to combine both representation models.
> This occurs, for example, when using the object-relational database model with UML.
>
> ###4.2 Generating database schemas from ontologies
> \[...]
>
> ### 4.3 Obtaining Ontologies from a database representations
> \[...]
>
> ### 4.4 Ontologies based databases
> \[...]
>
> -- \cite{martinez2011ontologies}
`[saved:martinez2011ontologies.pdf]`
[`[researchgate:publication:251332115]`](https://www.researchgate.net/publication/251332115)

```bibtex notes-library.bibtex +=
@article{martinez2011ontologies,
    author = {Martínez-Cruz, Carmen and Blanco, Ignacio and Vila, M.},
    year = {2011},
    month = {12},
    pages = {},
    title = {Ontologies versus relational databases: Are they so different? A comparison},
    volume = {38},
    journal = {Artificial Intelligence Review - AIR},
    doi = {10.1007/s10462-011-9251-9}
}
```

---

FIN.
