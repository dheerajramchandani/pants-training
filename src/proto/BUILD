protobuf_sources(
    name="protos",
    grpc=True,
)

# Added this target because otherwise Pants threw NoOwnerError.
python_distribution(
    name="proto-lib",
    dependencies=[":protos"],
    sdist=False,
    provides=python_artifact(
        name="proto-lib",
        version="0.1.0",
    )
)