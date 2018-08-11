load("@bazel_tools//tools/build_defs/pkg:pkg.bzl", "pkg_tar")

pkg_tar(
    name = "app1-dist",
    srcs = [
        "//src/main/java/io/github/hcoona:application1_deploy.jar",
    ],
    mode = "0755",
)

pkg_tar(
    name = "app2-dist",
    srcs = [
        "//src/main/java/io/github/hcoona:application1_deploy.jar",
    ],
    mode = "0755",
)
