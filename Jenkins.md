# Jenkins useful commands

List installed plugins (Use script console)

```groovy
Jenkins.instance.pluginManager.plugins.each{
  plugin -> 
    println ("${plugin.getShortName()}:${plugin.getVersion()}")
}
```

```
pipeline-build-step
github-pr-coverage-status
PrioritySorter
pipeline-model-declarative-agent
mask-passwords
docker-commons
sonar
locale
nodejs
jquery
variant
email-ext
ant
plain-credentials
jacoco
docker-workflow
nexus-artifact-uploader
git
rancher
github-branch-source
matrix-auth
build-monitor-plugin
pipeline-stage-step
github-api
github-oauth
conditional-buildstep
momentjs
display-url-api
workflow-job
workflow-basic-steps
ssh-slaves
scm-api
ace-editor
icon-shim
junit
pipeline-milestone-step
chromedriver
pipeline-model-extensions
antisamy-markup-formatter
pipeline-githubnotify-step
workflow-multibranch
github-organization-folder
jdk-tool
ldap
github
workflow-cps
pipeline-multibranch-defaults
jquery-ui
workflow-cps-global-lib
jsch
pipeline-stage-view
git-server
parameterized-trigger
external-monitor-job
apache-httpcomponents-client-4-api
ansicolor
run-condition
matrix-project
mailer
pipeline-input-step
resource-disposer
token-macro
branch-api
pipeline-rest-api
cucumber-reports
cloudbees-disk-usage-simple
discard-old-build
cloudbees-folder
pipeline-graph-analysis
gradle
sonar-quality-gates
gitlab-plugin
structs
workflow-scm-step
ws-cleanup
timestamper
jobConfigHistory
workflow-api
bouncycastle-api
durable-task
trilead-api
handlebars
workflow-durable-task-step
subversion
lockable-resources
ssh-credentials
git-client
jackson2-api
metrics
pipeline-stage-tags-metadata
cucumber-testresult-plugin
jquery-detached
pam-auth
credentials-binding
pipeline-model-api
javadoc
script-security
github-pullrequest
envinject
command-launcher
envinject-api
mapdb-api
disk-usage
config-file-provider
workflow-aggregator
credentials
role-strategy
greenballs
authentication-tokens
pipeline-github-lib
git-changelog
pipeline-model-definition
workflow-support
workflow-step-api
maven-plugin
skip-certificate-check
windows-slaves
```

## Node.js need to be installed and configured
- https://nodejs.org/en/
- npm config set proxy http://ip:port/ --global
- npm config set https-proxy http://ip:port/ --global 
- npm config set strict-ssl false --global
- npm config set registry http://registry.npmjs.org –-global

## Yarn need to be installed and configured
- npm install -g yarn
- yarn --version
- yarn config set strict-ssl false –global
- yarn config set proxy http://ip:port/ --global
- yarn config set https-proxy http://ip:port/ --global

## Environment variables need to be configured
- set HTTP_PROXY=http://ip:port/
- set HTTPS_PROXY=http://ip:port/


> ` mvn clean package -U -Ddockerfile.skip`

### If you get line separator error
- Go to root folder of the related project and type:
> `git config core.autocrlf`
> `yarn install`
