load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "homedir.go",
        "homedir_linux.go",
        "homedir_others.go",
    ],
    importmap = "github.com/GoogleCloudPlatform/docker-credential-gcr/v2/vendor/github.com/docker/docker/pkg/homedir",
    importpath = "github.com/docker/docker/pkg/homedir",
    visibility = ["//visibility:public"],
)
