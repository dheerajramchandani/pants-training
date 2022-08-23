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
        version="0.1.0",
    )
)

docker_image(
    name="docker",
    dependencies=[":server_source_code", "3rdparty:python_requirements"]
)

file(
    name="server_source_code",
    source="greeter_server.py",
)