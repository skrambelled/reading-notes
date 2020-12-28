# Django settings

There are many ways to set up your Django settings, each with their own pros and cons.

Some of the main issues to solve are that you may have different environments, such as a development environment and a production environment (and typically several layers of dev env). You might have sensitive data that you need to not expose, such as API tokens, DB passwords, and the Django SECRET_KEY. You also need to make it so that this information is available to your team, without introducing human error.

The best way to handle this is by using django-environ which gives us a .env file which is not shared to git, and a settings.py file for each of our django apps.

---

## SSH

Secure Shell is a secure replacement for telnet. SSH is encrypted, and provided a method for authentication. Linux and macOS can ssh directly from a terminal window. Windows users can use clients like Putty. You can then enter commands remotely from a client as if they were being entered directly on the host machine.

to open a ssh session in a terminal:

```bash
ssh {user}@{host}
```

This will prompt you for your password. Once entered properly, you are logged in!

## SSH encryption

There are 3 different ways SSH can encrypt transmitted data:

1. Symmetrical encryption
2. Asymmetrical encryption
3. Hashing

Symmetrical encryption means that both parties already have their key(s), and they are never transmitted to the other party.

Asymmetrivcal encryption uses a public/private key pair. The public key is used to encrypt the data, but only a private key can decrypt it.

Hashing is one directional, a hashed value cannot be unhashed (in theory). Hashes are used to verify that data being transferred is not tampered with.

SSH operates on port 22 by default.

[<-- Back](../README.md)
