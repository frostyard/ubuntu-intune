# ubuntu-intune
Container image meant to simplify the use of [Intune](https://www.microsoft.com/en-us/security/business/microsoft-intune) on [SNOSI](https://github.com/frostyard/snosi)

Currently, this container is based on Ubuntu 24.04 and includes:
* microsoft-identity-broker
* intune-portal
* unattended-upgrades
* Required PAM & security.d changes

Container images uploaded to the GHCR are signed with [cosign](https://github.com/sigstore/cosign) and can be validated against `cosign.pub` found in the root of this repository with:

`cosign verify --key cosign.pub ghcr.io/frostyard/ubuntu-intune:latest`
