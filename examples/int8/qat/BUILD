package(default_visibility = ["//visibility:public"])

cc_binary(
    name = "qat",
    srcs = [
        "main.cpp",
    ],
    copts = [
        "-pthread",
    ],
    linkopts = [
        "-lpthread",
    ],
    deps = [
        "//cpp:trtorch",
        "//examples/int8/benchmark",
        "//examples/int8/datasets:cifar10",
        "@libtorch",
        "@libtorch//:caffe2",
        "@tensorrt//:nvinfer",
    ],
)
