## Docker to save time and platform dependent errors
When one new team member was introduced to the project, at least one day was spent on setting up the environment. We found a solution to this with the use of `docker-compose`, we created our tailored Dockerfiles and described how they interacted with a simple YAML file. This saved us when our customer tried to run the full end to end test suite on their galera infrastructure, and it managed to bring down the *entire* cluster.

Essentially, a developer types “docker-compose up” and everything is set and ready to go. 

[Source](https://medium.com/the-node-js-collection/lessons-learned-one-year-with-node-js-and-the-enterprise-49f1adabf14a)

## TypeScript for solid code
TypeScript plugins will help to verify typescript code during development.
[Source](https://medium.com/the-node-js-collection/lessons-learned-one-year-with-node-js-and-the-enterprise-49f1adabf14a)

## Synk for security
[synk](https://snyk.io/) npm can find and help to fix vulnerabilities in dependencies
