package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_binary",
    "go_library",
    "go_test",
    "cgo_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "conditions.go",
        "helper.go",
    ],
    tags = ["automanaged"],
    deps = [
        "//pkg/api:go_default_library",
        "//pkg/api/errors:go_default_library",
        "//pkg/api/unversioned:go_default_library",
        "//pkg/apimachinery/registered:go_default_library",
        "//pkg/apis/apps:go_default_library",
        "//pkg/apis/batch:go_default_library",
        "//pkg/apis/extensions:go_default_library",
        "//pkg/client/clientset_generated/internalclientset/typed/apps/unversioned:go_default_library",
        "//pkg/client/clientset_generated/internalclientset/typed/batch/unversioned:go_default_library",
        "//pkg/client/clientset_generated/internalclientset/typed/core/unversioned:go_default_library",
        "//pkg/client/clientset_generated/internalclientset/typed/extensions/unversioned:go_default_library",
        "//pkg/client/restclient:go_default_library",
        "//pkg/util/wait:go_default_library",
        "//pkg/watch:go_default_library",
        "//plugin/pkg/client/auth:go_default_library",
    ],
)

go_test(
    name = "go_default_test",
    srcs = ["helper_test.go"],
    library = "go_default_library",
    tags = ["automanaged"],
    deps = [
        "//pkg/api:go_default_library",
        "//pkg/api/testapi:go_default_library",
        "//pkg/api/unversioned:go_default_library",
        "//pkg/apimachinery/registered:go_default_library",
        "//pkg/client/restclient:go_default_library",
        "//pkg/runtime:go_default_library",
    ],
)
