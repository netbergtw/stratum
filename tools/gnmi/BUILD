# Copyright 2018-present Open Networking Foundation
# SPDX-License-Identifier: Apache-2.0

load("@rules_cc//cc:defs.bzl", "cc_binary")
load("//bazel:rules.bzl", "STRATUM_DEFAULT_COPTS", "STRATUM_DEFAULT_LINKOPTS")

licenses(["notice"])  # Apache v2

package(
    default_visibility = ["//visibility:public"],
)

cc_binary(
    name = "gnmi-cli",
    srcs = ["gnmi_cli.cc"],
    copts = STRATUM_DEFAULT_COPTS,
    linkopts = STRATUM_DEFAULT_LINKOPTS,
    deps = [
        "//stratum/lib:utils",
        "@com_github_gflags_gflags//:gflags",
        "@com_github_grpc_grpc//:grpc++",
        "@com_github_openconfig_gnmi_proto//:gnmi_cc_grpc",
        "@com_github_openconfig_gnmi_proto//:gnmi_cc_proto",
        "@com_google_protobuf//:protobuf",
    ],
)
