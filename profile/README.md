# kognio

Java and Spring building blocks for working with knowledge graphs. The open ones
live here.

The name is a domain hack -- kogn.io, from Latin *cognoscere*, to know. That is
what the work is about: the part of a system that knows things, and keeping that
knowledge usable beyond the application that produced it.

## What is open here

- **[rdf-core](https://github.com/kogn-io/rdf-core)** -- technology-agnostic RDF
  data model, dataset and SHACL ports, and an RDF4J-backed adapter. The
  substrate the rest builds on. On Maven Central under `io.kogn.rdf`.

## How things are built here

W3C standards over homegrown DSLs. RDF, OWL, SHACL and SPARQL are boring in the
best sense: specified, stable, and surrounded by tooling nobody here has to
maintain. A proprietary format is quicker to invent and slower to live with -- a
parser, a validator, a query language and an ecosystem, all of it yours to keep
alive forever.

Boundaries that hold. The domain model stays independent of the engine that
stores it, so swapping the store is an adapter change rather than a rewrite.

## Who

Fred Hauschel, Java architect and developer in Munich, working on the seam
between ordinary Spring applications and knowledge-graph technology --
[hauschel.de/tech](https://www.hauschel.de/tech/).

## Licence

Apache-2.0 unless a repository states otherwise.
