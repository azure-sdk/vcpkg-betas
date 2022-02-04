# Azure SDK Beta Vcpkg Registry
This repo contains vcpkg registry for all Azure SDK releases - both stable releases and betas (unlike the [official vcpkg registry](https://github.com/microsoft/vcpkg), where only pre-stable beta and stable versions are being published, while post-first-stable betas are omitted to avoid having breaking changes).

## Usage
0. These instructions assume you know how to [get Azure SDK from the official vcpkg repo](https://github.com/Azure/azure-sdk-for-cpp#download--install-the-sdk). This document only documents the differences.
1. Download [`vcpkg-configuration.json`](https://github.com/azure-sdk/vcpkg-betas/blob/main/vcpkg-configuration.json) file from this repository, and put it into your vcpkg directory [^1].
2. Use `vcpkg` as usual.
3. Next time a release is available in this repo, get the updated `vcpkg-configuration.json` (step 1).

[^1]: In case you have other private registries configured in `vcpkg-configuration.json`, or have any other changes there that you don't want to be overwritten, manually merge the changes for the `vcpkg-betas` repo.
