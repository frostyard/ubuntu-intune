# ubuntu-intune
Container image for simplifying the use of [Intune](https://www.microsoft.com/en-us/security/business/microsoft-intune) on [SNOW Linux](https://github.com/frostyard/snosi) and other Linux distros with secure boot and full disk encryption.

Visit [intuneme](https://github.com/frostyard/intuneme) for a helpful CLI that makes use of this container.

This container is based on Ubuntu 24.04 LTS and includes:
* microsoft-identity-broker
* intune-portal
* unattended-upgrades
* Required PAM & security.d changes

Container images uploaded to the GHCR are signed with [cosign](https://github.com/sigstore/cosign) and can be validated with the `cosign.pub` file found in the root of this repository using:

`cosign verify --key cosign.pub ghcr.io/frostyard/ubuntu-intune:latest`
