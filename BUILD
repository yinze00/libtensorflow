cc_library(
    name = "tensorflow_cc",
    hdrs = glob(["include/**"]),
    strip_include_prefix = "include",
    srcs = [
        "lib/libtensorflow_cc.so.1.15.5"
    ],
    visibility = ["//visibility:public"],
)

cc_library(
    name = "tensorflow_framework",
    hdrs = glob(["include/**"]),
    strip_include_prefix = "include",
    srcs = [
        "lib/libtensorflow_framework.so.1.15.5"
    ],
    visibility = ["//visibility:public"],
)
