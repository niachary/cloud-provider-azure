load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["system_utils.go"],
    importmap = "sigs.k8s.io/cloud-provider-azure/vendor/k8s.io/kubernetes/test/e2e/system",
    importpath = "k8s.io/kubernetes/test/e2e/system",
    visibility = ["//visibility:public"],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
