### **Tutorial: Como Configurar e Usar o Compilador PAWN no Termux**

Olá, pessoal! Hoje vou mostrar como configurar e usar o compilador PAWN no Termux, tanto para SA-MP quanto para OPEN.MP. Vamos lá?

---

### **Passo 1: Atualizando as Bibliotecas**
Primeiro, precisamos garantir que todas as bibliotecas estejam atualizadas. Execute os seguintes comandos:

```bash
pkg update -y
pkg upgrade -y
```

---

### **Passo 2: Dando Permissão ao Termux**
Agora, vamos dar permissão ao Termux para acessar o armazenamento do seu dispositivo:

```bash
termux-setup-storage
```

---

### **Passo 3: Instalando o Compilador PAWN para SA-MP**
Para instalar o compilador PAWN atualizado, use os comandos abaixo:

```bash
curl https://raw.githubusercontent.com/termux-pawn/termux-pawn.github.io/refs/heads/1.2.1/install.sh | bash
pkg install -y pawncc
```

---

### **Passo 4: Instalando o Compilador PAWN para OPEN.MP (Opcional)**
Se você prefere usar o OPEN.MP, instale o compilador específico com este comando:

```bash
pkg install -y pawncc-11
```

---

### **Passo 5: Usando o Compilador PAWN**
Agora que tudo está instalado, vamos aprender a usar o compilador.

#### **Para SA-MP:**
```bash
pawncc [nome_do_arquivo.pwn]
```

#### **Para SA-MP com Tradução:**
```bash
pawncc -L2 [nome_do_arquivo.pwn]
```

#### **Para OPEN.MP:**
```bash
pawncc-11 [nome_do_arquivo.pwn]
```

#### **Para OPEN.MP com Tradução:**
```bash
pawncc-11 -L2 [nome_do_arquivo.pwn]
```

---

### **Dicas Extras para o Termux**

1. **Acessando a Pasta do Seu Gamemode:**
   Para entrar na pasta onde está seu gamemode, use o comando `cd`. Exemplo:
   ```bash
   cd /sdcard/Conteudo_Gamemode/Gamemode/gamemodes
   ```

2. **Compilando sem Poluir o Console:**
   Se quiser compilar sem deixar o console cheio de informações, use:
   ```bash
   clear && pawncc -L2 gamemode.pwn
   ```
   Ou, para OPEN.MP:
   ```bash
   clear && pawncc-11 -L2 gamemode.pwn
   ```

3. **Limpando o Console:**
   Para limpar o console, basta digitar:
   ```bash
   clear
   ```

---

### **Creditos**
Device Black: https://termux-pawn.github.io/
https://github.com/pawn-team/Termux-Pawn

### **Conclusão**
E é isso, pessoal! Agora você sabe como configurar e usar o compilador PAWN no Termux, tanto para SA-MP quanto para OPEN.MP. Se tiver alguma dúvida, deixe nos comentários! Não se esqueça de curtir, compartilhar e se inscrever no canal para mais tutoriais como este. Até a próxima! 🚀
