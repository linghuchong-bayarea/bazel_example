load("@io_bazel_rules_docker//python:image.bzl", "py_image")

package(default_visibility = ["//visibility:public"])

py_library(
    name = "lib",
    srcs = [
        "lib.py",
    ],
    deps = [],
)

py_image(
    name = "train",
    srcs = ["train.py"],
    main = "train.py",
    deps = [
        ":lib",
    ],
)
