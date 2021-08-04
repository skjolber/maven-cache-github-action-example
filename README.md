# maven-cache-github-action-example
Example Maven application.

Builds two jobs with github actions:

 * Maven with Github's [cache action](https://github.com/actions/cache)
 * Maven with [maven-cache-github-action](https://github.com/skjolber/maven-cache-github-action) or [maven-cache-github-action-beta](https://github.com/skjolber/maven-cache-github-action-beta)

# Simple spring project
The project has about 47 MB worth of dependencies, pulled directly from Maven Central.

# Experiment
Bump Spring version from 2.2.0 to 2.2.13.

# Results
Cache size results:

 * about __150 MB for Github's cache action__, 
 * about __50 MB for this action__ 
 
# Take-aways
The [maven-cache-github-action](https://github.com/skjolber/maven-cache-github-action) will see equivalent or a bit shorter build times. 








