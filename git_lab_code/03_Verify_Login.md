# Verify Login
- Once the SSH key is set up you need to add the private key into memory & test the connection, ensuring Github recognises it.
```
ssh-add ~/.ssh/github_project
ssh -T git@github.com
```
