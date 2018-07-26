# bazel-example-java #

Build Java project with [Google Bazel](https://www.bazel.build/).

## Generate single JAR package ##

Just append `_deploy.jar` to your `java_binary` target.

```
bazel build //app2:App2_deploy.jar
```

## How to use your Maven settings.xml ##

See https://github.com/bazelbuild/bazel/issues/3806 for further details.

### Option 1 ###

Use extension-skylark-based `maven_jar` rule:

```
load("@bazel_tools//tools/build_defs/repo:maven_rules.bzl",
  "maven_jar", "maven_dependency_plugin")
```

### Option 2 ###

Copy & specify the `settings.xml` from the rule `maven_server`.

```
maven_server(name="default", settings_file="//:settings.xml")
```
