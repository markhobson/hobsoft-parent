# Hobsoft Parent

Parent POM for [Hobsoft](http://www.hobsoft.org/) projects.

## Releasing

Prerequisites:

1. [Configure GPG key pair](https://central.sonatype.org/publish/requirements/gpg/)
1. [Configure Maven master password](https://maven.apache.org/guides/mini/guide-encryption.html#How_to_create_a_master_password)
1. [Configure Maven settings](https://central.sonatype.org/publish/publish-maven/#distribution-management-and-authentication) for server `sonatype-nexus-staging` with your [encrypted](https://maven.apache.org/guides/mini/guide-encryption.html#how-to-encrypt-server-passwords) OSSRH credentials

To release a new version:

1. `mvn release:clean release:prepare`
1. `mvn release:perform`
1. Enter GPG passphrase when prompted

## License

* [Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0.html)

[![CI](https://github.com/markhobson/hobsoft-parent/actions/workflows/ci.yml/badge.svg)](https://github.com/markhobson/hobsoft-parent/actions/workflows/ci.yml)
