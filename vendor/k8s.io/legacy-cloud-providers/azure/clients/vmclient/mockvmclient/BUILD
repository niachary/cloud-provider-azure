load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "doc.go",
        "interface.go",
    ],
    importmap = "sigs.k8s.io/cloud-provider-azure/vendor/k8s.io/legacy-cloud-providers/azure/clients/vmclient/mockvmclient",
    importpath = "k8s.io/legacy-cloud-providers/azure/clients/vmclient/mockvmclient",
    visibility = ["//visibility:public"],
    deps = [
        "//vendor/github.com/Azure/azure-sdk-for-go/services/compute/mgmt/2019-12-01/compute:go_default_library",
        "//vendor/github.com/golang/mock/gomock:go_default_library",
        "//vendor/k8s.io/legacy-cloud-providers/azure/retry:go_default_library",
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
