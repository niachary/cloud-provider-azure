package(default_visibility = ["//visibility:public"])

load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["metrics.go"],
    importmap = "sigs.k8s.io/cloud-provider-azure/vendor/k8s.io/component-base/metrics/prometheus/clientgo",
    importpath = "k8s.io/component-base/metrics/prometheus/clientgo",
    deps = [
        "//vendor/k8s.io/component-base/metrics/prometheus/clientgo/leaderelection:go_default_library",
        "//vendor/k8s.io/component-base/metrics/prometheus/restclient:go_default_library",
        "//vendor/k8s.io/component-base/metrics/prometheus/workqueue:go_default_library",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [
        ":package-srcs",
        "//staging/src/k8s.io/component-base/metrics/prometheus/clientgo/leaderelection:all-srcs",
    ],
    tags = ["automanaged"],
)
