genrule(
    name = "bar",
    srcs = [],
    outs = ["out.txt"],
    cmd = "echo > $OUT",
)

# Files in `//foo//bar:outs` should be inside `foo/bar`
# But here they appear in `foo` and cause a collision
filegroup(
    name = "outs",
    srcs = [":bar", "//foo/bar:outs"]
)

