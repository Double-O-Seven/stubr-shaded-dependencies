[![Actions Status](https://github.com/Double-O-Seven/stubr-shaded-dependencies/workflows/Java%20CI%20with%20Maven/badge.svg)](https://github.com/Double-O-Seven/stubr-shaded-dependencies/actions)
[![Release Version](https://img.shields.io/maven-central/v/ch.leadrian.stubr/stubr-shaded-dependencies.svg?label=release)](https://search.maven.org/search?q=g:ch.leadrian.stubr%20AND%20a:stubr-shaded-dependencies)

# stubr-shaded-dependencies

Shaded dependencies for [stubr](https://github.com/Double-O-Seven/stubr) to avoid version conflicts.

The following dependencies are shaded:

* `com.google.guava:guava:30.1.1-jre`

## Publishing steps

1. `eval "$(ssh-agent -s)"`
2. `ssh-add ~/.ssh/id_rsa`
3. `mvn release:clean release:prepare release:perform -B -e`
