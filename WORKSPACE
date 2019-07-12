workspace(name = "rules_java")

load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "bazel_federation",
    sha256 = "33222ab7bcc430f1ff1db8788c2e0118b749319dd572476c4fd02322d7d15792",
    strip_prefix = "bazel-federation-f0e5eda7f0cbfe67f126ef4dacb18c89039b0506",
    type = "zip",
    url = "https://github.com/bazelbuild/bazel-federation/archive/f0e5eda7f0cbfe67f126ef4dacb18c89039b0506.zip",  # 2019-09-30
)

load("@bazel_federation//:repositories.bzl", "rules_java_deps")

rules_java_deps()

load("@bazel_federation//setup:rules_java.bzl", "rules_java_setup")

rules_java_setup()

#
# Dependencies for development of rules_java itself.
#
load("//:internal_deps.bzl", "rules_java_internal_deps")

rules_java_internal_deps()

load("//:internal_setup.bzl", "rules_java_internal_setup")

rules_java_internal_setup()

maybe(
    http_archive,
    "host_jdk_linux",
    build_file = "@local_jdk//:BUILD.bazel",
    sha256 = "232b1c3511f0d26e92582b7c3cc363be7ac633e371854ca2f2e9f2b50eb72a75",
    strip_prefix = "zulu11.2.3-jdk11.0.1-linux_x64",
    urls = [
        "https://mirror.bazel.build/openjdk/azul-zulu11.2.3-jdk11.0.1/zulu11.2.3-jdk11.0.1-linux_x64.tar.gz",
    ],
)

maybe(
    http_archive,
    "host_jdk_macos",
    build_file = "@local_jdk//:BUILD.bazel",
    sha256 = "1edf366ee821e5db8e348152fcb337b28dfd6bf0f97943c270dcc6747cedb6cb",
    strip_prefix = "zulu11.2.3-jdk11.0.1-macosx_x64",
    urls = [
        "https://mirror.bazel.build/openjdk/azul-zulu11.2.3-jdk11.0.1/zulu11.2.3-jdk11.0.1-macosx_x64.tar.gz",
    ],
)

maybe(
    http_archive,
    "host_jdk_win",
    build_file = "@local_jdk//:BUILD.bazel",
    sha256 = "8e1e2b8347de6746f3fd1538840dd643201533ab113abc4ed93678e342d28aa3",
    strip_prefix = "zulu11.2.3-jdk11.0.1-win_x64",
    urls = [
        "https://mirror.bazel.build/openjdk/azul-zulu11.2.3-jdk11.0.1/zulu11.2.3-jdk11.0.1-win_x64.zip",
    ],
)

register_toolchains(
    "@rules_java//java/toolchains:all",
)
