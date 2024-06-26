Go generated proto packages
===========================

[![GoDoc](https://godoc.org/google.golang.org/genproto?status.svg)](https://godoc.org/google.golang.org/genproto)

```
代替： google.golang.org/genproto/...
```
> **WARNING(2023-05-26):** New submodules: upgrade before 2024-03-01 to avoid
> ambiguous import errors with
> [google.golang.org/genproto](https://pkg.go.dev/google.golang.org/genproto).
> See [#1015](https://github.com/googleapis/go-genproto/issues/1015) for more information.

> **IMPORTANT** This repository is currently experimental. The structure
> of the contained packages is subject to change. Please see the original
> source repositories (listed below) to find out the status of the each
> protocol buffer's associated service.

This repository contains the generated Go packages for common protocol buffer
types, and the generated [gRPC][1] code necessary for interacting with Google's gRPC
APIs.

The sources for the proto files used in this repository:

* [googleapis/googleapis][2]: the code in the `googleapis` is derived from this
  repo. The packages here contain types specifically for interacting with Google
  APIs.

Historically, the packages in the `protobuf` directory used to contain
generated code for certain well-known types hosted by [google/protobuf][3].
These types are now hosted by the [`google.golang.org/protobuf`][4] module
and type aliases are used to forward declarations in this module over to
declarations in the `protobuf` module.

[1]: http://grpc.io
[2]: https://github.com/googleapis/googleapis/
[3]: https://github.com/google/protobuf/
[4]: https://pkg.go.dev/mod/google.golang.org/protobuf
