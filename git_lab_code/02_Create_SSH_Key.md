# Create SSH Key
- This command allows you to generate a new SSH key to securely connect your local machine to Github.
- The use of the SSH key allows you to skip using a username & password each time.
```
ssh-keygen -t ed25519 -C "<EMAIL>" -f ~/.ssh/github_project
cat ~/.ssh/github_project.pub ssh-ed25519 <SSH KEY> <EMAIL>
```
