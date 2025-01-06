# WSL Github SSH Guide
1. Navigate to the User Directory:
```bash
cd ~
```
**OR**
```bash
cd /home/[User]
```

2. Create a **.ssh** file:
```bash
sudo mkdir .ssh
```

3. Set your global github credentials:
```bash
git config --global user.email "email"
git config --global user.name "name"
```

4. Execute Following Commands:
```bash
sudo ssh-keygen -o -t rsa -C "email"
```
5. Enter following for the options:
    - Enter file in which to save the key (/root/.ssh/id_rsa): /home/[user]/.ssh/id_rsa
    - Enter passphrase (empty for no passphrase): (Press Enter)
    - Enter same passphrase again: (Press Enter)

```bash
sudo chmod 400 ~/.ssh/id_rsa
cat ~/.ssh/id_rsa.pub
```

6. Copy the ssh key.
7. In your github profile setting navigate to the **SSH And GPG Keys**.
8. Click on **New SSH key**, give a name to the key and paste the key there.