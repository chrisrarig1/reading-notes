# API Deployment

## Best Practices

- *Different environments*: Each environment has its own specific settings. It is necessary to approach the environments to keep all Django setting configs
- *Sensitive data*: A secret key is given with the project as well as DB passwords and tokens. These should not be shared
- *Sharing settings between team members*: Develop an approach to eliminate human error. Especially when adding 3rd party api's
- *Django settings are a Python code*: It gives you a lot of flexibility, but can also be a problem – instead of key-value pairs, settings.py can have a very tricky logic

## 12 Factors

1. Codebase
2. Dependencies
3. Config
4. Backing services
5. Build, release, run
6. Processes
7. Port binding
8. Concurrency
9. Disposability
10. Dev/prod parity
11. Logs
12. Admin processes

## django-environ

- Perfect place to keep confidential info
- `import environ`
- Naming:
  - `DEBUG=True`
  - `DATABASE_URL=postgres://user:password@db.example.com:5432/production_db?sslmode=require`

## SSH

- *SSH*: Secure Shell Protocol, is a remote administration protocol that allows users to access, control, and modify their remote servers over the internet

- *3 Parts*: `ssh {user}@{host}`
  - `user`: represents the account you want access to
  - `host`: refers to the computer you want access to

### Different Encryption Techniques

- *Symmetric Encryption*: is a form of encryption where a secret key is used for both encryption and decryption
- *Asymmetrical Encryption*: uses two separate keys for encryption and decryption: Public and Private keys
- *Hashing*: It generates a unique value of a fixed length for each input that shows no clear trend which can be exploited. This makes them practically impossible to reverse

### Authenticating the User

- *The final step*: The authentication process is when information given by the user is passed to the server. Upon confirmation a key is then sent back to the user allowing access

# Useful Links

- [Configuring Django Settings: Best Practices](https://djangostars.com/blog/configuring-django-settings-best-practices/)
- [How Does SSH Work: Everything You Need to Know](https://www.hostinger.com/tutorials/ssh-tutorial-how-does-ssh-work)