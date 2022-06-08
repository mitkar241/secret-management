# README
---
`Lyft`’s approach to secrets management resulted in a tool called `Confidant`. Lyft keeps it short and sweet on the description: “Your secret keeper. Stores secrets in DynamoDB, encrypted at rest.”

In describing the problem Lyft was trying to solve with Confidant, Lyft explains that with all the new internal and external services, keeping track of keys and secrets became a very laborious process:

> "As Lyft has grown, we’ve added numerous services to our infrastructure. These services have credentials to internal services and external services, SSL keys, and other types of secrets. Each of these services has multiple environments, and to insulate these environments from each other, they have a version of each of these secrets for each environment. In many cases some of these secrets may be shared across a few services. Given a large number of services, this leads to a very large number of credentials.
The rotation of these secrets can be a laborious process, especially credentials for external services, since a large number of external services don’t have rotation methods that can be done without some amount of downtime and coordination. Coordination of the rotation of secrets became a difficult and time-consuming process for us pretty early on, and we knew the problem would only get worse as we added more internal services and more external dependencies."
