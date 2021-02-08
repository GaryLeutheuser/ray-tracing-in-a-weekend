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

cc_library(
    name = "ray",
    hdrs = ["ray.h"],
    deps = [
        ":vec3",
    ],
)

cc_library(
    name = "hittable",
    hdrs = ["hittable.h"],
    deps = [
        ":ray",
    ],
)

cc_library(
    name = "sphere",
    hdrs = ["sphere.h"],
    deps = [
        ":hittable",
        ":vec3",
    ],
)

cc_library(
    name = "hittable_list",
    hdrs = ["hittable_list.h"],
    deps = [
        ":hittable",
    ],
)

cc_library(
    name = "rtweekend",
    hdrs = ["rtweekend.h"],
    deps = [
        ":ray",
        ":vec3",
    ],
)

cc_library(
    name = "camera",
    hdrs = ["camera.h"],
    deps = [
        ":rtweekend",
    ],
)

cc_binary(
    name = "main",
    srcs = ["main.cc"],
    deps = [
        ":rtweekend",
        ":color",
        ":sphere",
        ":hittable_list",
        ":camera",
    ],
)
