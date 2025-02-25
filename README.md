# maven-cache-github-action-example
Example Maven application.

Builds two jobs with github actions:

 * Maven with Github's [cache action](https://github.com/actions/cache)
 * Maven with [maven-cache-github-action](https://github.com/skjolber/maven-cache-github-action) or [maven-cache-github-action-beta](https://github.com/skjolber/maven-cache-github-action-beta)

# Simple spring project
The project has about 47 MB worth of dependencies, pulled directly from Maven Central.

# Results

 * Github's cache action downloads on each pom.xml change  
 * [maven-cache-github-action](https://github.com/skjolber/maven-cache-github-action) or [maven-cache-github-action-beta](https://github.com/skjolber/maven-cache-github-action-beta) is able to restore the cache on pom.xml changes
 
# Take-aways
Github's cache read/write speeds is very good. 

The [maven-cache-github-action](https://github.com/skjolber/maven-cache-github-action) __will probably result in a bit shorter build times__, as cache speed > maven central speed. If you rely on a third party artifact repository, then probably cache speed >> repo speed.











