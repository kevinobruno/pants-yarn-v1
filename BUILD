files(
    name="package_config",
    sources=[
        "tsconfig.json",
    ],
)

files(
    name="code",
    sources=["**/*.ts"],
)

package_json(
    name="root",
    dependencies=[
        ":package_config",
        ":code",
    ],
    scripts=[
        node_build_script(
            entry_point="build",
            output_directories=["src"],
        ),
    ],
)
