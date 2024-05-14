load("@io_bazel_rules_go//go:def.bzl", "go_library")

go_library(
    name = "go_default_library",
    srcs = [
        "clientauth.go",
        "sts_exchange.go",
    ],
    importmap = "github.com/GoogleCloudPlatform/docker-credential-gcr/v2/vendor/golang.org/x/oauth2/google/internal/stsexchange",
    importpath = "golang.org/x/oauth2/google/internal/stsexchange",
    visibility = ["//vendor/golang.org/x/oauth2/google:__subpackages__"],
    deps = ["//vendor/golang.org/x/oauth2:go_default_library"],
)
