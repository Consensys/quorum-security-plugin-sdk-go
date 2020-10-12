# Go SDK for Quorum security plugins

## Quickstart

```shell
# account plugin sdk
go get github.com/ConsenSys/quorum-security-plugin-sdk-go/proto

# plugin initialization sdk
go get github.com/ConsenSys/quorum-security-plugin-sdk-go/proto_common

# mocks for testing
go get github.com/ConsenSys/quorum-security-plugin-sdk-go/mock_proto
```

## Overview

[Quorum's pluggable architecture](https://docs.goquorum.consensys.net/en/latest/Concepts/Plugins/Plugins/) allows for a Quorum node to be extended with additional functionality.

`security` plugins [add security to Quorum's RPC API](https://docs.goquorum.consensys.net/en/latest/HowTo/Use/JSON-RPC-API-Security/).

The communication between Quorum and a `security` plugin uses gRPC.

This SDK can be used to develop Go `security` plugins that fulfill Quorum's gRPC `security` plugin interface.  It provides the necessary Go types and methods for starting a new gRPC server, initializing a new plugin, and for handling Quorum gRPC requests.

***This repo is auto-updated***

*The [quorum-plugin-definitions](https://github.com/ConsenSys/quorum-plugin-definitions) project defines the `security` plugin gRPC API.  A [GitHub Actions workflow](.github/workflows/run.yml) updates the SDK whenever quorum-plugin-definitions is altered.*
