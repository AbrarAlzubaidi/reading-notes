# Django Settings Best Practices
## Managing Django Settings: Issues

- Each environment can have its own specific settings. Sensitive data. 
- You have SECRET_KEY in each Django project. On top of this there can be DB passwords and tokens for third-party APIs like Amazon or Twitter. This data cannot be stored in VCS.
- You need a general approach to eliminate human error when working with the settings. 
- Django settings are a Python code. It gives you a lot of flexibility, but can also be a problem – instead of key-value pairs, settings.py can have a very tricky logic.
- **settings_local.py is not in VCS, so you can lose some of your Django environment settings.**
- **Writing code using os.environ could require additional effort to handle errors. It’s better to use django-environ instead.**

## Django Settings: Best practices
- Keep settings in environment variables.
- Write default values for production configuration (excluding secret keys and tokens).
- Don’t hardcode sensitive settings, and don’t put them in VCS.
- Split settings into groups: Django, third-party, project.
- Follow naming conventions for custom (project) settings.

------

# SSH

- **SSH**, or Secure Shell, is a remote administration protocol that allows users to control and modify their remote servers over the Internet.

- It provides a mechanism for authenticating a remote user, transferring inputs from the client to the host, and relaying the output back to the client.

## How Does SSH Work

    The SSH command consists of 3 distinct parts:

        ssh {user}@{host}

- ssh: instructs your system that you want to open an encrypted (Secure Shell Connection)
- user: the account you want to access
- host: refers to the computer you want to access.This can be an IP Address or a domain name

### There are three different encryption technologies used by SSH:

- Symmetrical encryption: a form of encryption where a **secret key is used for both encryption and decryption** of a message by both the client and the host. Effectively, any one possessing the key can decrypt the message being transferred. Symmetrical encryption is often called **shared key** or **shared secret encryption**. There is usually only one key that is used, or sometimes a pair keys where one key can easily be calculated using the other key.

- Asymmetrical encryption: it uses two **separate** keys for encryption and decryption. **These two keys are known as the public key and the private key**. Together, both these keys form a public-private key pair.

- Hashing: One-way-hash functions differ from the above two forms of encryption in the sense that they are never meant to be decrypted. They generate a unique value of a fixed length for each input that shows no clear trend which can exploited. This makes them practically impossible to reverse. **SSH uses hashes** to verify the authenticity of messages. This is done using **HMACs**, or Hash-based Message Authentication Codes. This ensures that the command received is not tampered with in any way.

## How Does SSH Work with These Encryption Techniques

- by making use of a client-server model to allow for authentication of two remote systems and encryption of the data that passes between them.

- Both the client and the server agree on a very large prime number, which of course does not have any factor in common. This prime number value is also known as the seed value.
- Next, the two parties agree on a common encryption mechanism to generate another set of values by manipulating the seed values in a specific algorithmic manner. These mechanisms, also known as encryption generators, perform large operations on the seed.
- Both the parties independently generate another prime number. This is used as a secret private key for the interaction.
- This newly generated private key, with the shared number and encryption algorithm, is used to compute a public key which is distributed to the other computer.
- then use their personal private key, the other machine’s shared public key and the original prime number to create a final shared key. This key is independently computed by both computers but will create the same encryption key on both sides.
- Now that both sides have a shared key, they can symmetrically encrypt the entire SSH session. The same key can be used to encrypt and decrypt messages.

***resources***

1. [django-settings-best-practices](https://djangostars.com/blog/configuring-django-settings-best-practices/)
2. [SSH](https://www.hostinger.com/tutorials/ssh-tutorial-how-does-ssh-work)