[![Actions Status](https://github.com/Double-O-Seven/stubr-shaded-dependencies/workflows/Java%20CI%20with%20Maven/badge.svg)](https://github.com/Double-O-Seven/stubr-shaded-dependencies/actions)

# stubr-shaded-dependencies
Shaded dependencies for [stubr](https://github.com/Double-O-Seven/stubr) to avoid version conflicts.

The following dependencies are shaded:
* `com.google.guava:guava:29.0-jre`

## Publishing steps

1. `eval "$(ssh-agent -s)"`
2. `ssh-add ~/.ssh/id_rsa`
3. `mvn release:clean release:prepare release:perform -B -e`
