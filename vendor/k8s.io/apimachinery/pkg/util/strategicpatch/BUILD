package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "errors.go",
        "meta.go",
        "patch.go",
        "types.go",
    ],
    importmap = "sigs.k8s.io/cloud-provider-azure/vendor/k8s.io/apimachinery/pkg/util/strategicpatch",
    importpath = "k8s.io/apimachinery/pkg/util/strategicpatch",
    deps = [
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1/unstructured:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/json:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/util/mergepatch:go_default_library",
        "//vendor/k8s.io/apimachinery/third_party/forked/golang/json:go_default_library",
        "//vendor/k8s.io/kube-openapi/pkg/util/proto:go_default_library",
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
        "//staging/src/k8s.io/apimachinery/pkg/util/strategicpatch/testing:all-srcs",
    ],
    tags = ["automanaged"],
)
