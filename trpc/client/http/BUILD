licenses(["notice"])

package(default_visibility = ["//visibility:public"])

cc_library(
    name = "http_service_proxy",
    srcs = ["http_service_proxy.cc"],
    hdrs = ["http_service_proxy.h"],
    deps = [
        "//trpc/client:rpc_service_proxy",
        "//trpc/codec:client_codec_factory",
        "//trpc/codec/http:http_client_codec",
        "//trpc/common/future",
        "//trpc/stream/http:http_client_stream",
        "//trpc/util/http:request",
        "//trpc/util/http:response",
        "//trpc/util/log:logging",
        "@com_github_tencent_rapidjson//:rapidjson",
    ],
)

cc_library(
    name = "http_stream_proxy",
    srcs = ["http_stream_proxy.cc"],
    hdrs = ["http_stream_proxy.h"],
    deps = [
        "//trpc/client:service_proxy",
        "//trpc/codec/http:http_protocol",
        "//trpc/stream/http/async:stream_reader_writer",
    ],
)

