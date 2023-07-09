# FlowIt Monorepo

Welcome to FlowIt Monorepo! Here's you'll find all the source code for the flowIt app alongside its backing services and utilities. Primarily this concerns:

1. The mobile web application (JS, React Native + Expo)
2. The backend API and Web views (Python, Django)


## Getting started

To get started, cd into either application and follow their setup README:s.


## Tooling

There is no advanced tooling or monorepo cohesion, this is mainly just a single repository to keep it simple. That said, you do have an obvious inter dependency between mobile application and backend server. It can be helpful to run both simulatenously. 

## Deployment and CI/CD

Every application is deployed as a standalone application with its own associated deployment process. In the *.github* folder, these workflows are detailed. As a developer, you do not need to manually deploy, but can instead rely on following the contribution flow via pull request, and have your changes be automatically deployed.


### Deployment environments

FlowIt uses a single environment as the production environment (exposed to customers) for simplicities sake. Any changes merged to the *main* branch will be deployed.


### Contributing

To contribute, start by downloading the repository via git and making your feature branch. Do not push to master.

```bash
# download repo
git clone git@github.com:flowit-uk/apps.git flowit

# create feature branch
git checkout -B feature/new-super-cool-feature
```
