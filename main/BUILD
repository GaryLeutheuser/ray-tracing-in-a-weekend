cc_library(
    name = "vec3",
    hdrs = ["vec3.h"],
)

cc_library(
    name = "color",
    hdrs = ["color.h"],
    deps = [
        ":vec3",
    ],
)



cc_binary(
    name = "main",
    srcs = ["main.cc"],
    deps = [
        ":vec3",
        ":color",
    ],
)
