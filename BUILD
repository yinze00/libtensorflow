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

cc_library(
    name = "tensorflow",
    hdrs = glob(["include/**"]),
    strip_include_prefix = "include",
    srcs = [
        "lib/libtensorflow_cc.so.1",
        "lib/libtensorflow_framework.so.1"
    ],
    visibility = ["//visibility:public"],
)

cc_library(
    name = "cc_op_gen_main",
    srcs = [
        "lib/libcc_op_gen_main.so",
    ],
    # linkopts = [
    #     "-Lexternal/tensorflow/lib -ltensorflow_cc"
    # ],
    deps = [
        ":tensorflow"
    ],
    visibility = ["//visibility:public"],
)