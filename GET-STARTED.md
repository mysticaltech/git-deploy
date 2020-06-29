# Get Started with git-deploy

## 1. Generating a new SSH key
1. Paste the text below, substituting in your GitHub email address.
```
$ ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

2. When you're prompted to "Enter a file in which to save the key," press Enter. This accepts the default file location.

3. At the prompt, type a secure passphrase.

4. Get the public key by pasting the text below. Copy the public key.
```
cat path\to\your\key\generated
```

5. Go to your GitHub Settings -> SSH & GPG Keys -> New SSH key -> paste your key

## 2. Setup the deployment script by following instruction in README
