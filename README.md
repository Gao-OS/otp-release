# Build `otp-release` from source

[![Build Linux amd64 standalone otp-release](https://github.com/Gao-OS/otp-release/actions/workflows/build-otp-release-linux-amd64.yaml/badge.svg)](https://github.com/Gao-OS/otp-release/actions/workflows/build-otp-release-linux-amd64.yaml)
[![Build Linux arm64 standalone otp-release](https://github.com/Gao-OS/otp-release/actions/workflows/build-otp-release-linux-arm64.yaml/badge.svg)](https://github.com/Gao-OS/otp-release/actions/workflows/build-otp-release-linux-arm64.yaml)
---
Supplies prebuilt erlang otp release

## Custom ERTS Builds for [Burrito](https://github.com/burrito-elixir/burrito)

Precompiled builds of Erlang Runtime System Application, ERTS for the Burrito project.

- `[os: :darwin, cpu: :x86_64]`
- `[os: :darwin, cpu: :aarch64]`
- `[os: :linux, cpu: :x86_64]`
- `[os: :linux, cpu: :aarch64]`
- `[os: :windows, cpu: :x86_64]`


This is the custom build of ERTS, you're able to override the precompiled binaries on a per target basis by setting custom_erts to the path of your ERTS build:

```elxiir
targets: [
  linux_arm: [
    os: :linux,
    cpu: :x86_64,
    custom_erts: "https://github.com/Gao-OS/otp-release/releases/download/main/OTP-27.1.2-linux-amd64.tar.gz"
  ]
]
```
