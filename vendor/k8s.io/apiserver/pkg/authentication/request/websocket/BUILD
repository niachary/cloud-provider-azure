package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = ["protocol.go"],
    importmap = "sigs.k8s.io/cloud-provider-azure/vendor/k8s.io/apiserver/pkg/authentication/request/websocket",
    importpath = "k8s.io/apiserver/pkg/authentication/request/websocket",
    deps = [
        "//vendor/k8s.io/apiserver/pkg/authentication/authenticator:go_default_library",
        "//vendor/k8s.io/apiserver/pkg/util/wsstream:go_default_library",
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
)
