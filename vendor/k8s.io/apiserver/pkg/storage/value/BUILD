package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "metrics.go",
        "transformer.go",
    ],
    importmap = "sigs.k8s.io/cloud-provider-azure/vendor/k8s.io/apiserver/pkg/storage/value",
    importpath = "k8s.io/apiserver/pkg/storage/value",
    deps = [
        "//vendor/google.golang.org/grpc/status:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/errors:go_default_library",
        "//vendor/k8s.io/component-base/metrics:go_default_library",
        "//vendor/k8s.io/component-base/metrics/legacyregistry:go_default_library",
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
        "//staging/src/k8s.io/apiserver/pkg/storage/value/encrypt/aes:all-srcs",
        "//staging/src/k8s.io/apiserver/pkg/storage/value/encrypt/envelope:all-srcs",
        "//staging/src/k8s.io/apiserver/pkg/storage/value/encrypt/identity:all-srcs",
        "//staging/src/k8s.io/apiserver/pkg/storage/value/encrypt/secretbox:all-srcs",
    ],
    tags = ["automanaged"],
)
