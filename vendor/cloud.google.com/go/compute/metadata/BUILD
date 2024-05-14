load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "metadata.go",
        "retry.go",
        "retry_linux.go",
    ],
    importmap = "github.com/GoogleCloudPlatform/docker-credential-gcr/v2/vendor/cloud.google.com/go/compute/metadata",
    importpath = "cloud.google.com/go/compute/metadata",
    visibility = ["//visibility:public"],
)
