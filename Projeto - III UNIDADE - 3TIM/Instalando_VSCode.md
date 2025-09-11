# 📘 Guia de Instalação do Visual Studio Code no Linux Mint (Xfce / Cinnamon / Mate)

Este guia mostra como instalar o **Visual Studio Code** no Linux Mint utilizando o repositório oficial da Microsoft.

---

## 🔹 1. Atualizar o sistema
Abra o terminal e rode:

```bash
sudo apt update && sudo apt upgrade -y
```

---

## 🔹 2. Adicionar o repositório oficial da Microsoft

1. Instale os pacotes necessários:
```bash
sudo apt install wget gpg -y
```

2. Baixe e adicione a chave de assinatura da Microsoft:
```bash
wget -qO- https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > packages.microsoft.gpg
```

3. Mova a chave para o local correto:
```bash
sudo install -o root -g root -m 644 packages.microsoft.gpg /etc/apt/trusted.gpg.d/
```

4. Adicione o repositório do VS Code:
```bash
echo "deb [arch=amd64,arm64,armhf] https://packages.microsoft.com/repos/code stable main" | sudo tee /etc/apt/sources.list.d/vscode.list
```

---

## 🔹 3. Instalar o VS Code
Agora basta atualizar os pacotes e instalar:

```bash
sudo apt update
sudo apt install code -y
```

---

## 🔹 4. Abrir o VS Code
No terminal:

```bash
code
```

Ou pesquise **Visual Studio Code** no menu do Linux Mint.

---

## 🔹 5. (Opcional) Atalhos úteis

- Abrir pasta no VS Code direto do terminal:
```bash
code nome-da-pasta
```

- Abrir arquivo específico:
```bash
code arquivo.py
```
