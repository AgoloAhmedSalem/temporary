licenses(["notice"])  # Apache 2.0

package(
    default_visibility = [
    "//tensorflow_serving:internal"
    ]
)

cc_binary(
    name = 'extract_spans.so',
    srcs = [
        "./coref_kernels.cc",
    ],
    linkshared = 1,
)


cc_library(
    name = 'extract_spans.so',
    visibility = ["//visibility:public"],
    srcs = [
        "./coref_kernels.cc",
    ],
    alwayslink = 1,
    deps = [
        "@org_tensorflow//tensorflow/core:framework",
    ]
)