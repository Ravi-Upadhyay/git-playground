## Initial Setup

This guide is for initial setup of Git on the developer machine from scratch.

---

## Index

- Setting up global config
- Setting up SSH
- To do 

---

## Setting up global config

Setting up global config ensures that one do not need to enter details each time they push

```
git config --global user.name <user-name>
git config --global user.email <user-email>
```

---

## Setting up SSH

Setting up SSH has following workflow

1. Check if development machine already have ssh keys
2. Create ssh key pair at development machine
3. Add private key (from key pair generated in step 2) to ssh agent running on the developer machine 
4. Add public key (from key pair generated in step 2) to the github 

[Github Docs - connect with SSH](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account?tool=webui)

---

## To do

- Create some aliases for commonly used functionalities
- Create workflow for settings of a project

---