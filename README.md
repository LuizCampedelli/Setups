# WSL Ubuntu

## In powershell:

```bash
wsl --update
```

```bash
wsl --install -d ubuntu
```

```bash
wsl --set-default-version 2
```

```bash
wsl --install --web-download
```

```bash
sudo apt update && sudo apt upgrade -y && sudo apt install ubuntu-standard -y
```


Crie um arquivo chamado .wslconfig na raiz da sua pasta de usuário (C:\Users\<seu_usuario>)
Create a file named .wslconfig in the root folder of yor user (C:\Users\<your_user_name>)

```bash
memory=8GB
processors=4
swap=2GB
```

#############

Remove WSL

```bash
wsl --list
wsl --unregister ubuntu
```

# AWS CLI

```bash
sudo apt update
sudo apt install curl
sudo apt install unzip
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
rm aws -rf
rm awscliv2.zip -f
```

# Kubectl 

```bash
sudo apt-get update
sudo apt-get install -y apt-transport-https ca-certificates curl

curl -fsSL https://pkgs.k8s.io/core:/stable:/v1.30/deb/Release.key | sudo gpg --dearmor -o /etc/apt/keyrings/kubernetes-apt-keyring.gpg

echo 'deb [signed-by=/etc/apt/keyrings/kubernetes-apt-keyring.gpg] https://pkgs.k8s.io/core:/stable:/v1.30/deb/ /' | sudo tee /etc/apt/sources.list.d/kubernetes.list

sudo apt-get update
sudo apt-get install -y kubectl
```

# Helm

```bash
curl https://baltocdn.com/helm/signing.asc | gpg --dearmor | sudo tee /usr/share/keyrings/helm.gpg > /dev/null

sudo apt-get install apt-transport-https --yes

echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/helm.gpg] https://baltocdn.com/helm/stable/debian/ all main" | sudo tee /etc/apt/sources.list.d/helm-stable-debian.list

sudo apt-get update
sudo apt-get install helm
```

# Github

```bash
git config --global user.name "nome"
git config --global user.email "e-mail"
```

Public key

```bash
ssh-keygen -t rsa -b 4096 -o -a 128 -C "e-mail"
sudo cat /home/anderson/.ssh/id_rsa.pub
```

