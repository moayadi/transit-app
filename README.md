# Encryption as a Service Example

This repo seeks to provide an example that demonstrates how to protect sensitive data using [HashiCorp Vault](http://hashicorp.com/products/vault/).

The [Transit secrets engine](https://www.vaultproject.io/docs/secrets/transit) in HashiCorp Vault provides an API that can be used to perform a variety of cryptographic operations, such as encryption, decryption, signing, hashing, and HMAC. It can also be used for secure key generation, or providing a unified method for random number generation.

The [Transform secrets engine](https://www.vaultproject.io/docs/secrets/transform) in HashiCorp Vault provides an API that can be used to perform secure data transformation and tokenization against a provided input value. This can be used to implement format preserving encryption as well as masking of sensitive data. 

This repo contains a simple CRUD app that can integrate with Vault to protect customer records.

![](demo.png?raw=true)
