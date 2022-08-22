pex_binary(
    name="greeter_server",
    entry_point="greeter_server.py",
)

python_sources()

python_distribution(
    name="grpc-server",
    dependencies=[":server"],
    sdist=False,
    provides=python_artifact(
        name="grpc-server",
    )
)

docker_image(
    name="docker",
)