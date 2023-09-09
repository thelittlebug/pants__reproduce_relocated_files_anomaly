# cocomo-bazel

python_sources(
    name = "src",
    dependencies = [
        "src/tuhls/core",
    ],
)

pex_binary(
    name = "manage_dev_pex",
    dependencies = [":src"],
    entry_point = "manage.py",
    execution_mode = "venv",
    layout = "loose",
)
