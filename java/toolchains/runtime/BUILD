package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load("@local_config_platform//:constraints.bzl", "HOST_CONSTRAINTS")

toolchain(
    name = "local_jdk",
    exec_compatible_with = HOST_CONSTRAINTS,
    target_compatible_with = HOST_CONSTRAINTS,
    toolchain = "@local_jdk//:jdk",
    toolchain_type = "@rules_java//java/toolchains:runtime_toolchain_type",
)
