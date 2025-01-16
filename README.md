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
