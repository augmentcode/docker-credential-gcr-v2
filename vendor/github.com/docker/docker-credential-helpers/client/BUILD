load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "client.go",
        "command.go",
    ],
    importmap = "github.com/GoogleCloudPlatform/docker-credential-gcr/v2/vendor/github.com/docker/docker-credential-helpers/client",
    importpath = "github.com/docker/docker-credential-helpers/client",
    visibility = ["//visibility:public"],
    deps = ["//vendor/github.com/docker/docker-credential-helpers/credentials:go_default_library"],
)
