package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = ["interface.go"],
    importmap = "sigs.k8s.io/cloud-provider-azure/vendor/k8s.io/client-go/informers/rbac",
    importpath = "k8s.io/client-go/informers/rbac",
    deps = [
        "//vendor/k8s.io/client-go/informers/internalinterfaces:go_default_library",
        "//vendor/k8s.io/client-go/informers/rbac/v1:go_default_library",
        "//vendor/k8s.io/client-go/informers/rbac/v1alpha1:go_default_library",
        "//vendor/k8s.io/client-go/informers/rbac/v1beta1:go_default_library",
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
        "//staging/src/k8s.io/client-go/informers/rbac/v1:all-srcs",
        "//staging/src/k8s.io/client-go/informers/rbac/v1alpha1:all-srcs",
        "//staging/src/k8s.io/client-go/informers/rbac/v1beta1:all-srcs",
    ],
    tags = ["automanaged"],
)
