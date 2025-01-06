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
sudo chmod 400 ~/.ssh/id_rsa
cat ~/.ssh/id_rsa.pub
```
5. Copy the ssh key.
6. In your github profile setting navigate to the **SSH And GPG Keys**.
7. Click on **New SSH key**, give a name to the key and paste the key there.