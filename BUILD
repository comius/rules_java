licenses(["notice"])

exports_files(["LICENSE"])

filegroup(
    name = "distribution",
    srcs = [
        "BUILD",
        "LICENSE",
    ] + glob([
        "*.bzl",
    ]),
    visibility = ["@//distro:__pkg__"],
)

exports_files(
    ["WORKSPACE"],
    visibility = ["//visibility:public"],
)
