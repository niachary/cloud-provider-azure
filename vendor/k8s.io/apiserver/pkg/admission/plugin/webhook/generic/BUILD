load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "conversion.go",
        "interfaces.go",
        "webhook.go",
    ],
    importmap = "sigs.k8s.io/cloud-provider-azure/vendor/k8s.io/apiserver/pkg/admission/plugin/webhook/generic",
    importpath = "k8s.io/apiserver/pkg/admission/plugin/webhook/generic",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/k8s.io/api/admission/v1:go_default_library",
        "//vendor/k8s.io/api/admission/v1beta1:go_default_library",
        "//vendor/k8s.io/api/admissionregistration/v1:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/api/errors:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//vendor/k8s.io/apimachinery/pkg/runtime/schema:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/admission:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/admission/initializer:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/admission/plugin/webhook:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/admission/plugin/webhook/config:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/admission/plugin/webhook/namespace:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/admission/plugin/webhook/object:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/admission/plugin/webhook/rules:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/util/webhook:go_default_library",
        "//vendor/k8s.io/client-go/informers:go_default_library",
        "//vendor/k8s.io/client-go/kubernetes:go_default_library",
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
    srcs = [":package-srcs"],
    tags = ["automanaged"],
    visibility = ["//visibility:public"],
)
