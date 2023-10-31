package(name = "see")

    load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

    # Python-FastAPI

    http_archive(
        name = "python_fastapi",
        url = "https://github.com/tiangolo/fastapi/archive/refs/heads/master.zip",
        strip_prefix = "fastapi-master",
    )

    # Flutter

    http_archive(
        name = "flutter",
        url = "https://storage.googleapis.com/flutter_infra/flutter.zip",
        strip_prefix = "flutter",
        build_file = "@flutter//tools/build_defs/repo.bzl",
    )