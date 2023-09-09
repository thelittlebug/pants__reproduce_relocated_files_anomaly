# cocomo-bazel
resources(
    #dependencies = [":wrapped_files"],
    sources = ["**/*"],
)

experimental_wrap_as_python_sources(
    name = "wrapped_files",
    inputs = [":relocated_files"],
    outputs = ["**/*"]
)

relocated_files(
    name = "relocated_files",
    src = "src/js_libs",
    dest = "src/tuhls/core/static",
    files_targets = ["src/js_libs/alpinejs.3.10.3.min.js"],
)
