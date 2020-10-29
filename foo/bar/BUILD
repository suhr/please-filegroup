genrule(
    name = "bar",
    srcs = [],
    outs = ["out.txt"],
    cmd = "echo > $OUT",
)

filegroup(
    name = "outs",
    srcs = [":bar"],
    visibility = ["PUBLIC"],
)

