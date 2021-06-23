Streamlining DBS retrieval and sync of core data

Ingestion repo is organized as a monolith composed of nested dependencies covering a large surface area including product summary, details, payment orders, transactions. 

Targeted improvements in service of the following outcomes:
- Reduce dependency between processing and sync of independent core banking features
- De-risk single unit of deployment as there are differences in maturity and completeness of processing components 
- Enable failure isolation and reduce maintenance burden
- Improve feature buildout cadence
- Incorporate domain knowledge gained through the course of the program
- Enable transition to flexible event triggers and workflows

Suggestions 
Split into individual processors orchestrated through local events, starting with payment orders and transactions

Payment-orders-processor
