## Project with versioning and tagging

### Basic use case

```
./gradlew bumpVersionFile gitCommit gitTag
```

- version.properties file will be bumped
- commit will be created
- tag will be created

### With git push

```
./gradlew bumpVersionFile gitCommit gitTag gitPush
```

In addition to versioning and tagging, we also trigger git push. 
Requires GH_WRITE_TOKEN env variable exported OR command line user with write permissions.