# LOD_auto_mapper
This repo will be the demo space for LOD mapping in large triplestores that have many different ontologies in them.

## Key repos

- https://github.com/mapping-commons/sssom | standard to adhere to when making the mapping
- https://github.com/vliz-be-opsci/k-gap | platform to initially gather the LOD that is used to do the mapping to.

## Workflow

1. Gather LOD first in triplestore.
2. Make a named graph dipicting all the possibe paths and relation between the triples (predicates2predicates, predicate2objectstype).
3. Gather ?s ?p ?o for all the ?p in the triplestore. This will be the web of explanations about each triple in another named graph.
4. Do vector analysis / LLM analysis on all these triples in the semantic predicate explanation graph in the SSSOM standard way.
5. Use the results of the named graph made in 2,3,4 as context to answer Natural language questions to make sparql queries.
