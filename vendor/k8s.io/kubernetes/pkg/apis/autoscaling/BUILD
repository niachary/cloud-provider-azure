package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "annotations.go",
        "doc.go",
        "helpers.go",
        "register.go",
        "types.go",
        "zz_generated.deepcopy.go",
    ],
    importpath = "k8s.io/kubernetes/pkg/apis/autoscaling",
    deps = [
        "//pkg/apis/core:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/api/resource:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/runtime/schema:go_default_library",
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
        "//pkg/apis/autoscaling/fuzzer:all-srcs",
        "//pkg/apis/autoscaling/install:all-srcs",
        "//pkg/apis/autoscaling/v1:all-srcs",
        "//pkg/apis/autoscaling/v2beta1:all-srcs",
        "//pkg/apis/autoscaling/v2beta2:all-srcs",
        "//pkg/apis/autoscaling/validation:all-srcs",
    ],
    tags = ["automanaged"],
)