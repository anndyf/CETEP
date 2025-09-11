# 🐧 Guia de Comandos de Navegação no Linux

Este guia reúne os comandos básicos para navegar e se localizar no terminal Linux.  

---

## 📂 1. Mostrar diretório atual
```bash
pwd
```
Exibe o caminho completo da pasta em que você está.

---

## 📂 2. Listar arquivos e pastas
```bash
ls
```
Lista os arquivos do diretório atual.

Opções úteis:
- `ls -l` → lista detalhada (permissões, dono, tamanho, data).
- `ls -a` → mostra também arquivos ocultos.
- `ls -lh` → lista detalhada com tamanhos legíveis (KB, MB, GB).

---

## 📂 3. Mudar de diretório
```bash
cd nome_da_pasta
```

Exemplos:
- `cd /home/usuario/Documentos` → vai para a pasta Documentos.
- `cd ..` → volta uma pasta.
- `cd ~` → vai para o diretório pessoal do usuário.
- `cd /` → vai para a raiz do sistema.

---

## 📂 4. Criar pastas e arquivos
```bash
mkdir nova_pasta
```
Cria uma nova pasta.

```bash
touch arquivo.txt
```
Cria um arquivo vazio.

---

## 📂 5. Copiar, mover e remover
- Copiar arquivo:
```bash
cp arquivo.txt /caminho/de/destino/
```

- Mover ou renomear arquivo:
```bash
mv arquivo.txt /caminho/de/destino/
```

- Remover arquivo:
```bash
rm arquivo.txt
```

- Remover pasta e conteúdo:
```bash
rm -r nome_da_pasta
```

---

## 📂 6. Ver conteúdo de arquivos
```bash
cat arquivo.txt
```
Mostra todo o conteúdo do arquivo.

```bash
less arquivo.txt
```
Permite rolar o conteúdo com as setas.

```bash
head arquivo.txt
```
Mostra as 10 primeiras linhas.

```bash
tail arquivo.txt
```
Mostra as 10 últimas linhas.

---

## 📂 7. Histórico de comandos
```bash
history
```
Mostra a lista dos últimos comandos executados.

---

## 📂 8. Atalhos úteis no terminal
- `Ctrl + C` → interrompe o comando atual.
- `Ctrl + L` → limpa a tela (igual a `clear`).
- `↑` e `↓` → navega pelos últimos comandos digitados.
- `Tab` → autocompleta nomes de arquivos e pastas.

---
