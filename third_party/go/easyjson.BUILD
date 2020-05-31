package(default_visibility = ["@//visibility:public"])

load("@//third_party:go/build.bzl", "external_go_package")

external_go_package(
    base_pkg = "github.com/mailru/easyjson",
    deps = [
        "@easyjson//:jlexer",
        "@easyjson//:jwriter",
    ],
)

external_go_package(
    name = "jlexer",
    base_pkg = "github.com/mailru/easyjson",
    deps = [
        "@go_intern_strings//:intern",
    ],
    exclude_srcs = [
        "bytestostr_nounsafe.go",
    ],
)

external_go_package(
    name = "jwriter",
    base_pkg = "github.com/mailru/easyjson",
    deps = [
        "@easyjson//:buffer",
    ],
)

external_go_package(
    base_pkg = "github.com/mailru/easyjson",
    name = "buffer",
)
