load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["accessors.go"],
    importmap = "sigs.k8s.io/cloud-provider-azure/vendor/k8s.io/apiserver/pkg/admission/plugin/webhook",
    importpath = "k8s.io/apiserver/pkg/admission/plugin/webhook",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/k8s.io/api/admissionregistration/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/labels:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/util/webhook:go_default_library",
        "//vendor/k8s.io/client-go/rest:go_default_library",
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
        "//staging/src/k8s.io/apiserver/pkg/admission/plugin/webhook/config:all-srcs",
        "//staging/src/k8s.io/apiserver/pkg/admission/plugin/webhook/errors:all-srcs",
        "//staging/src/k8s.io/apiserver/pkg/admission/plugin/webhook/generic:all-srcs",
        "//staging/src/k8s.io/apiserver/pkg/admission/plugin/webhook/initializer:all-srcs",
        "//staging/src/k8s.io/apiserver/pkg/admission/plugin/webhook/mutating:all-srcs",
        "//staging/src/k8s.io/apiserver/pkg/admission/plugin/webhook/namespace:all-srcs",
        "//staging/src/k8s.io/apiserver/pkg/admission/plugin/webhook/object:all-srcs",
        "//staging/src/k8s.io/apiserver/pkg/admission/plugin/webhook/request:all-srcs",
        "//staging/src/k8s.io/apiserver/pkg/admission/plugin/webhook/rules:all-srcs",
        "//staging/src/k8s.io/apiserver/pkg/admission/plugin/webhook/testcerts:all-srcs",
        "//staging/src/k8s.io/apiserver/pkg/admission/plugin/webhook/testing:all-srcs",
        "//staging/src/k8s.io/apiserver/pkg/admission/plugin/webhook/util:all-srcs",
        "//staging/src/k8s.io/apiserver/pkg/admission/plugin/webhook/validating:all-srcs",
    ],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
