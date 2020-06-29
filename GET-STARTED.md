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
* Install via composer
```
composer require senangprint/git-deploy:dev-master
```

## 3. Setup git on production server
1. Initialize git repo
```
git init
```

2. Add remote origin
```
git remote add origin <github repo ssh url>
```

3. Set upstream
```
git branch --set-upstream-to=origin/master master
```

4. Pull origin
```
git pull
```


## References
- https://medium.com/better-programming/how-to-automatically-deploy-from-github-to-server-using-webhook-79f837dcc4f4
- https://stackoverflow.com/questions/32056324/there-is-no-tracking-information-for-the-current-branch
