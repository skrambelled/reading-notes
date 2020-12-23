# JSON Web Tokens

JSON Web tokens are a standardized way for two parties to securely transfer JSON data using a public/private key.

They can be encrypted to enforce privacy and they can also be used to verify integrity of data being transferred.

A JWT has:

- header
- payload
- signature

## header

The header has two components. It lists the type of web token it is, which in this case is a `JWT`, and it also lists which signing algorithm was used, such as `HS256`

## Payload

The payload has the claims, which can be public, private, or registered.

## Signature

The signature is used to verify intergrity of the data, using a secrect key that has been hashed.

---

We can use JWT for a single signp-on web app, where a user signs on and all of their subsequent web requests will include a JWT for authentication.


[<-- Back](../README.md)
