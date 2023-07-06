Dependency Track Bash / ZSH client
==================================

An OpenApi codegen-generated client for [Dependency Track](https://dependencytrack.org/) in Bash / ZSH.

# How to use

```bash
export DTRACK_HOST=https://your.dtrack.host
export DTRACK_APIKEY=yourApiKey
dtrack getVersion
```

# How to develop

Use the provided Gradle wrapper to generate the code :

```bash
./gradlew openApiGenerate
```

You can then go to ``build/generated`` to build the Docker image :

```bash
docker build -t dtrack-cli .
```
and run it :
```bash
docker run -it dtrack-cli
```

# Development Roadmap

* Integrate image building in Gradle with the JIB plugin
* Customize container image to add extra tooling (e.g. JQ)


