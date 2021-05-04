# Infrastructure

> **Adopt** - The default choice when selecting technologies, currently in use in production
>
> **Assess**  - Technologies that we believe may be valuable, and are currently being assessed to understand their value and impact.
>
> **Hold** - Technologies in hold must no longer be used for new development

## Adopt
### AWS EC2
Cloud compute gives us the flexibility of scaling to demand. Our initial migration was a very similar set up to what we had previously. We will continue to look at improving this to gain the full benefits.

### Teamcity + octopus deploy
Mature build and deployment tooling

### Docker for testing
We are seeing benefits of using on-demand testing environments for quick and reliable acceptance testing.

### AWS S3
For static storage. 

### AWS Cloudfront
CDN to go in front of S3 etc. 


## Assess
### Infrastructure-as-code tools - Terraform
These tools could help us to reduce environment-specific issues, and improve documentation. We have picked terraform as it is the best supported cross platform tool. Although parts of scripts would need to be rewritten, it provides a consistent base across platforms (rather than using cloudformation etc)

### Server-less platforms (AWS Lambda)
We need to understand the potential that server-less platforms can offer in reducing operational overhead of server management with a small operations team. Currently testing in MAS. For simple logic, can be sensible. If it is complicated, just use a sever. Part of the assessment will be defining when it is and isn't sensible to use.

As part of this we are trialling API gateway.

### Azure
Currently looking at what capabilities this can provide us

### Things other than IIS. 
On a project by project basis we will assess if things should be self hosted.


## Hold
### Containers in production
We've not seen enough benefits in running docker in production over our existing Teamcity -> Octopus deploy -> AWS EC2 infrastructure.
