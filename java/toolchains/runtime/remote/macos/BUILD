package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@rules_java//java/constraints:constraints.bzl",
    "MACOS_CONSTRAINTS",
    "REMOTE_JDK10_CONSTRAINTS",
    "REMOTE_JDK11_CONSTRAINTS",
    "REMOTE_JDK12_CONSTRAINTS",
    "REMOTE_JDK9_CONSTRAINTS",
)

toolchain(
    name = "jdk9",
    exec_compatible_with = MACOS_CONSTRAINTS + REMOTE_JDK9_CONSTRAINTS,
    target_compatible_with = MACOS_CONSTRAINTS + REMOTE_JDK9_CONSTRAINTS,
    toolchain = "@remote_jdk9_macos//:jdk",
    toolchain_type = "@rules_java//java/toolchains:runtime_toolchain_type",
)

toolchain(
    name = "jdk10",
    exec_compatible_with = MACOS_CONSTRAINTS + REMOTE_JDK10_CONSTRAINTS,
    target_compatible_with = MACOS_CONSTRAINTS + REMOTE_JDK10_CONSTRAINTS,
    toolchain = "@remote_jdk9_macos//:jdk",
    toolchain_type = "@rules_java//java/toolchains:runtime_toolchain_type",
)

toolchain(
    name = "jdk11",
    exec_compatible_with = MACOS_CONSTRAINTS + REMOTE_JDK11_CONSTRAINTS,
    target_compatible_with = MACOS_CONSTRAINTS + REMOTE_JDK11_CONSTRAINTS,
    toolchain = "@remote_jdk9_macos//:jdk",
    toolchain_type = "@rules_java//java/toolchains:runtime_toolchain_type",
)

toolchain(
    name = "jdk12",
    exec_compatible_with = MACOS_CONSTRAINTS + REMOTE_JDK12_CONSTRAINTS,
    target_compatible_with = MACOS_CONSTRAINTS + REMOTE_JDK12_CONSTRAINTS,
    toolchain = "@remote_jdk9_macos//:jdk",
    toolchain_type = "@rules_java//java/toolchains:runtime_toolchain_type",
)
