package(
    default_visibility = ["//src:__subpackages__"]
)

java_binary(
    name = "application1",
    srcs = [
        "App1.java",
    ],
    deps = [
        ":library2",
    ],
    visibility = [
        "//:__pkg__",
    ],
)

java_binary(
    name = "application2",
    srcs = [
        "App2.java",
    ],
    deps = [
        ":library1",
    ],
    visibility = [
        "//:__pkg__",
    ],
)

java_library(
    name = "library1",
    srcs = [
        "Library1.java",
    ],
    deps = [
        "@com_google_guava_guava//jar",
    ],
)

java_library(
    name = "library2",
    srcs = [
        "Library2.java",
    ],
)
