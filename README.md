# maven-cache-github-action-example
Example Maven application.

Builds two jobs with github actions:

 * Maven with Github's [cache action](https://github.com/actions/cache)
 * Maven with [maven-cache-github-action](https://github.com/skjolber/maven-cache-github-action)
 * Maven with [maven-cache-github-action-beta](https://github.com/skjolber/maven-cache-github-action-beta)

# Simple spring project
About 47 MB worth of dependencies, pulled directly from Maven Central.

# Results
Build time is equivalent, except from when the pom.xml file changes. Then [maven-cache-github-action](https://github.com/skjolber/maven-cache-github-action) has a few seconds shorter build time, because it is able to restore the dependency cache from the previous build. The difference between the two jobs will vary depending on how good the fallback cache is / how much was changed, and the bandwidth of you repository store.









