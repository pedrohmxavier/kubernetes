load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = ["scanner.go"],
    importmap = "k8s.io/kubernetes/vendor/github.com/hashicorp/hcl/json/scanner",
    importpath = "github.com/hashicorp/hcl/json/scanner",
    visibility = ["//visibility:public"],
    deps = ["//vendor/github.com/hashicorp/hcl/json/token:go_default_library"],
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
