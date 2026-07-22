# kognio

Open building blocks for RDF and knowledge-graph systems in the Java and Spring
world.

The premise: a knowledge graph is not a storage detail you bolt on at the end.
It is a modelling decision, and it deserves the same care as the rest of the
domain model -- an explicit vocabulary, validation you can run in CI, and a
boundary between the model and the engine that stores it.

So everything here is cut hexagonally. The domain model is technology-agnostic;
the triple store sits behind a port. Replacing the engine is an adapter change,
not a rewrite.

## Building blocks

- **[rdf-core](https://github.com/kogn-io/rdf-core)** -- technology-agnostic RDF
  data model, dataset and SHACL ports, and an RDF4J-backed adapter. The
  substrate the rest builds on. Released to Maven Central under `io.kogn.rdf`.

## Why W3C standards

RDF, OWL, SHACL and SPARQL are boring in the best sense: specified, stable, and
surrounded by tooling nobody here has to maintain. A proprietary DSL would be
quicker to invent and slower to live with -- a parser, a validator, a query
language and an ecosystem, all of it yours to keep alive forever.

## Licence

Apache-2.0 unless a repository states otherwise.
