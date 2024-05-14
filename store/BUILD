load("@io_bazel_rules_go//go:def.bzl", "go_library", "go_test")

go_library(
    name = "go_default_library",
    srcs = ["store.go"],
    importpath = "github.com/GoogleCloudPlatform/docker-credential-gcr/v2/store",
    visibility = ["//visibility:public"],
    deps = [
        "//config:go_default_library",
        "//util:go_default_library",
        "//vendor/github.com/docker/docker-credential-helpers/credentials:go_default_library",
        "//vendor/golang.org/x/oauth2:go_default_library",
        "//vendor/golang.org/x/oauth2/google:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = [
        "store_integration_test.go",
        "store_unit_test.go",
    ],
    embed = [":go_default_library"],
    deps = select({
        "@io_bazel_rules_go//go/platform:aix": [
            "//vendor/golang.org/x/oauth2:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:android": [
            "//vendor/golang.org/x/oauth2:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:darwin": [
            "//vendor/golang.org/x/oauth2:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:dragonfly": [
            "//vendor/golang.org/x/oauth2:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:freebsd": [
            "//vendor/golang.org/x/oauth2:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:illumos": [
            "//vendor/golang.org/x/oauth2:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:ios": [
            "//vendor/golang.org/x/oauth2:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:js": [
            "//vendor/golang.org/x/oauth2:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:linux": [
            "//vendor/golang.org/x/oauth2:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:netbsd": [
            "//vendor/golang.org/x/oauth2:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:openbsd": [
            "//vendor/golang.org/x/oauth2:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:plan9": [
            "//vendor/golang.org/x/oauth2:go_default_library",
        ],
        "@io_bazel_rules_go//go/platform:solaris": [
            "//vendor/golang.org/x/oauth2:go_default_library",
        ],
        "//conditions:default": [],
    }),
)
