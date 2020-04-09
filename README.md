# Encryption As A Service Example

This repo seeks to provide an example that demonstrates how to protect sensitive data using Hashicorp Vault.  Encryption as a service, or the transit secret engine, provides an API that can be used to perform a variety of cryptographic operations such as encryption and decryption, signing, hashing, HMAC, etc.  It has other uses as well including secure key generation, providing a unified method for random number generation, and other things.

This repo contains a simple CRUD app that can integrate with Vault to protect customer records.

To be continued...  For now look in the setup directory.

Andy create a token with no TTL for demo purposes
Could otherwise use approle + vault agent to populate the token in config.ini
vault token create -policy=transit-app-example -ttl=8760h

path "enterprise/west/transit/customer-key" {
  capabilities = ["read"]
}

path "enterprise/west/transit/archive-key" {
  capabilities = ["read"]
}

careful to run the webserver from backend folder

Known Issues:
need to be able to delete
you lose the nav bar at around 1100-1200 pixels wide