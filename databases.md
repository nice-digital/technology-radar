# Databases

> **Adopt** - The default choice when selecting technologies, currently in use in production
>
> **Assess**  - Technologies that we believe may be valuable, and are currently being assessed to understand their value and impact.
>
> **Hold** - Technologies in hold must no longer be used for new development

## Adopt
### Elastic Search	
Preferred solution for full-text search and analytics.

### Microsoft SQL Server	
Preferred solution where the data is relational.

### Redis	
Preferred solution as a key-value store.

### AWS S3	
Blob storage.

## Assess
### Mongo DB / DocumentDB	
Used for a few systems at NICE: Medtech, Docs/Appraisals and NICE docs (retired). Also assess use when combined with Meteor (as used with Medtech).

### CosmosDB	

## Hold
### RavenDB 
A lack of community and skills market make this a risky technology to continue using, despite its good points. Breaking changes between versions make it difficult to upgrade.

### Stardog
Graph database & RDF store used in the BNF build process.
