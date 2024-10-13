# test-workflow

CI/CD Workflows:
- Automated testing
- Automated deployment
- SDLC 

CI (Continuous Integration)
CD (Continuous Deployment)


CI/CD Technologies:
- GitHub Actions
- Jenkins
- GitLab CI/CD
- CircleCI
- Travis CI


## Github Actions

Goal: A workflow to build, test and deploy a Go application.


Workflow -> A series of jobs
Job -> A set of tasks

A series of sequential jobs. Jobs can be run in parallel or sequentially.
A job is a set of steps.

Workflow => A workflow to build, test and deploy a Go application.

Job => Build, Test, Deploy => 3 jobs

Build Job:
- Checkout code
- Build the application (Dockerfile)
- Push image to a registry


Actions are lego blocks that can be used to build a workflow.

A workflow can be called by different events.
- Push to a repository
- Schedule (cron job)
- Manually
- External event


### Build
[x] Dockerfile
[ ] Registry

### 