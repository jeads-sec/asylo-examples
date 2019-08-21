#
# Copyright 2019 Asylo authors
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#

load("@com_google_asylo//asylo/bazel:copts.bzl", "ASYLO_DEFAULT_COPTS")

licenses(["notice"])

# An implementation of ApplicationConfig() that returns an EnclaveConfig with
# an SGX local assertion authority config.
cc_library(
    name = "redis_enclave_config",
    srcs = ["redis_enclave_config.cc"],
    visibility = ["//visibility:public"],
    deps = [
        "@com_google_asylo//asylo:enclave_cc_proto",
        "@com_google_asylo//asylo/identity:descriptions",
        "@com_google_asylo//asylo/identity:enclave_assertion_authority_config_cc_proto",
        "@com_google_asylo//asylo/identity/sgx:sgx_local_assertion_authority_config_cc_proto",
        "@com_google_asylo//asylo/util:logging",
    ],
)