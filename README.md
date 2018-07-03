# Credentials

This repo wants to show, by example, bad practices that can be avoided
regarding to the storage and usage of credentials and keystore files.

The branch organisation for the repo will be named like: 

- **master** : Base project without signing configs + README.

- **bad** : Plain text credentials in ``build.gradle`` file. Keystore file in the same repository.

- **not_that_bad** : Plain text credentials stored in the user's ``gradle.properties``. Keystore file in the same repository. 

- **quite_better** : Plain text credentials stored in the user's ``gradle.properties``. Keystore file in the user's gradle directory.

- **better** : Credentials exposed as ENV variables. Keystore file fetched from another repository.

- **actually_better** : Encrypted credentials stored in a local Vault-like storage system. Keystore file fetched from another repository.

- **optimal** : Usage of a ``configServer`` for the storage of the encrypted credentials. Keystore file fecthed from another repository.