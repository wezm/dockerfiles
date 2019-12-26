# diesel\_cli Docker image

This image is use to build the diesel CLI for use in my CI pipeline.

Build the image, then build the CLI:

    docker run --rm -it -v $(pwd)/out:/out diesel_cli cargo install --root /out diesel_cli --no-default-features --features postgres --version 1.4.0
