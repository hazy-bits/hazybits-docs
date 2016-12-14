# AWS Services
So far we use the following AWS services:

 * `Lambda Functions` - main power behind the solution. Small blocks that perform
 processing operations and can be composed in a number of ways, maintaining high
 scalability.
 * `Step Functions` - new workflow engine that allows to orchestrate lambda
 functions and build complex workflows with concurrent execution, retries, and
 error handling.
 * `S3` - intermediate storage for images and extracted metadata.
 * `IoT` - pubsub infrastructure, mainly to enable web socket communication
 channel between clients and cloud infrastructure.
