package(default_visibility = ["//visibility:public"])

licenses(["notice"])

load(
    "@rules_java//java/constraints:constraints.bzl",
    "JAVAC10_LANGUAGE8_CONSTRAINTS",
    "JAVAC11_LANGUAGE8_CONSTRAINTS",
    "JAVAC12_LANGUAGE8_CONSTRAINTS",
    "JAVAC9_LANGUAGE8_CONSTRAINTS",
    "MACOS_CONSTRAINTS",
)

toolchain(
    name = "java_tools",
    exec_compatible_with = MACOS_CONSTRAINTS,
    target_compatible_with = MACOS_CONSTRAINTS,
    toolchain = "@remote_java_tools_darwin//:toolchain",
    toolchain_type = "@rules_java//java/toolchains:toolchain_type",
)

toolchain(
    name = "javac9_language8",
    exec_compatible_with = MACOS_CONSTRAINTS + JAVAC9_LANGUAGE8_CONSTRAINTS,
    target_compatible_with = MACOS_CONSTRAINTS + JAVAC9_LANGUAGE8_CONSTRAINTS,
    toolchain = "@remote_java_tools_javac10_macos//:toolchain",
    toolchain_type = "@rules_java//java/toolchains:toolchain_type",
)

toolchain(
    name = "javac10_language8",
    exec_compatible_with = MACOS_CONSTRAINTS,  #+ JAVAC10_LANGUAGE8_CONSTRAINTS,
    target_compatible_with = MACOS_CONSTRAINTS,  #+ JAVAC10_LANGUAGE8_CONSTRAINTS,
    toolchain = "@remote_java_tools_javac10_macos//:toolchain",
    toolchain_type = "@rules_java//java/toolchains:toolchain_type",
)

toolchain(
    name = "javac11_language8",
    exec_compatible_with = MACOS_CONSTRAINTS + JAVAC11_LANGUAGE8_CONSTRAINTS,
    target_compatible_with = MACOS_CONSTRAINTS + JAVAC11_LANGUAGE8_CONSTRAINTS,
    toolchain = "@remote_java_tools_javac11_macos//:toolchain",
    toolchain_type = "@rules_java//java/toolchains:toolchain_type",
)

toolchain(
    name = "javac12_language8",
    exec_compatible_with = MACOS_CONSTRAINTS + JAVAC12_LANGUAGE8_CONSTRAINTS,
    target_compatible_with = MACOS_CONSTRAINTS + JAVAC12_LANGUAGE8_CONSTRAINTS,
    toolchain = "@remote_java_tools_javac12_macos//:toolchain",
    toolchain_type = "@rules_java//java/toolchains:toolchain_type",
)
