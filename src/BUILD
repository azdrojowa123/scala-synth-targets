load("@io_bazel_rules_scala//scala:scala.bzl", "scala_library", "scala_test", "scala_test_suite")

scala_test_suite(
    name = "tests",
    srcs = glob(
        include = ["scala/**/*.scala"],
        exclude = ["scala/com/example/inside/*.scala"],
    ),
    deps = [
        ":lib00",
    ],
)

scala_library(
    name = "lib00",
    srcs = glob(["scala/com/example/inside/*.scala"]),
)

scala_library(
    name = "lib3",
    srcs = glob(["scala/com/example/inside2/*.scala"]),
)
