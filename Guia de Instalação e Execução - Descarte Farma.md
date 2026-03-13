#  Guia de Instalação e Execução - Descarte Farma

##  Pré-requisitos

Antes de começar, certifique-se de que você tem instalado em seu computador:

- **Node.js** (versão 16 ou superior) - [Download aqui](https://nodejs.org/)
- **Git** (opcional, mas recomendado) - [Download aqui](https://git-scm.com/)

---

##  Passo 1: Baixar o Projeto

### Opção A: Baixar do Google Drive (ZIP)

1. Acesse o link do Google Drive fornecido
2. Clique em **"Download"** para baixar o arquivo `descarte-farma-prototype.zip`
3. Extraia o arquivo em seu computador:
   - **Windows**: Clique direito → **"Extrair tudo"**
   - **Mac/Linux**: Abra o terminal e execute: `unzip descarte-farma-prototype.zip`

### Opção B: Clonar do GitHub (se já estiver no repositório)

```bash
git clone https://github.com/seu-usuario/descarte-farma.git
cd descarte-farma-prototype
```

---

##  Passo 2: Abrir o Terminal na Pasta do Projeto

### No Windows (CMD - Recomendado)

1. Pressione `Win + R`
2. Digite `cmd` e pressione **Enter**
3. Navegue até a pasta do projeto:
   ```bash
   cd C:\Users\seu-usuario\Documents\caminho-do-projeto\descarte-farma-prototype
   ```

### No Windows (PowerShell)

1. Abra o **PowerShell** como Administrador
2. Se receber erro de permissão, execute:
   ```powershell
   Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
   ```
3. Confirme digitando `Y` e pressionando **Enter**
4. Navegue até a pasta:
   ```bash
   cd C:\Users\seu-usuario\Documents\caminho-do-projeto\descarte-farma-prototype
   ```

### No Windows (Git Bash)

1. Clique direito na pasta do projeto
2. Selecione **"Git Bash Here"**
3. Você já estará na pasta correta

### No Mac/Linux

1. Abra o **Terminal**
2. Navegue até a pasta:
   ```bash
   cd ~/caminho-do-projeto/descarte-farma-prototype
   ```

---

##  Passo 3: Instalar as Dependências

Execute um dos comandos abaixo no terminal:

### Instalação Padrão (Recomendado)

```bash
npm install
```

### Se Receber Erro na Instalação Padrão

Use este comando com a flag `--legacy-peer-deps`:

```bash
npm install --legacy-peer-deps
```

### Se Ainda Assim Não Funcionar

Execute os comandos abaixo em sequência:

```bash
npm cache clean --force
npm install
```

---

##  Passo 4: Executar o Projeto

Após a instalação das dependências, execute:

```bash
npm run dev
```

Você verá uma mensagem no terminal como:

```
➜  Local:   http://localhost:5173/
```

---

##  Passo 5: Acessar o Protótipo

1. Abra seu navegador (Chrome, Firefox, Edge, Safari, etc.)
2. Acesse: **http://localhost:5173/**
3. Pronto! O protótipo do **Descarte Farma** estará rodando! 

---

##  O que Você Verá

O protótipo inclui:

• **Tela de Navegação (Mapa)** - Visualize os pontos de coleta no mapa interativo  
• **Tela de Detalhes** - Informações detalhadas com simulação de visão 360°  
• **Guia Rápido** - Instruções sobre como descartar medicamentos  
• **Design Responsivo** - Interface em forma de celular  
• **Cores Oficiais** - Vermelho Vinho (#800020) e Branco  
• **Navegação Fluida** - Transições suaves entre as telas  

---

##  Troubleshooting (Solução de Problemas)

### Erro: "npm: comando não encontrado"

**Solução:** Node.js não está instalado. [Baixe e instale aqui](https://nodejs.org/)

### Erro: "EACCES: permission denied"

**Solução (Mac/Linux):** Execute com `sudo`:
```bash
sudo npm install
```

### Erro: "Cannot find module"

**Solução:** Delete a pasta `node_modules` e execute novamente:
```bash
rm -rf node_modules
npm install
```

### Porta 5173 já está em uso

**Solução:** Use uma porta diferente:
```bash
npm run dev -- --port 3000
```

---

##  Estrutura do Projeto

```
descarte-farma-prototype/
├── client/
│   ├── src/
│   │   ├── pages/
│   │   │   └── Home.tsx          (Componente principal)
│   │   ├── index.css             (Estilos globais)
│   │   └── App.tsx               (Configuração da aplicação)
│   ├── index.html                (Arquivo HTML principal)
│   └── public/                   (Arquivos estáticos)
├── package.json                  (Dependências do projeto)
├── vite.config.ts                (Configuração do Vite)
└── README.md                     (Documentação do projeto)
```

---

##  Próximos Passos

Após rodar o projeto localmente, você pode:

1. **Personalizar o design** - Edite os arquivos em `client/src/`
2. **Adicionar funcionalidades** - Implemente novas features
3. **Fazer deploy** - Hospede em plataformas como Vercel, Netlify ou GitHub Pages
4. **Compartilhar no GitHub** - Faça push do seu código para o repositório

---

##  Suporte

Se encontrar problemas:

1. Verifique se Node.js está instalado: `node --version`
2. Verifique se npm está instalado: `npm --version`
3. Tente limpar o cache: `npm cache clean --force`
4. Delete `node_modules` e `package-lock.json`, depois instale novamente

---

## 📄 Licença

Este projeto é de propriedade exclusiva do autor. Todos os direitos são reservados.
Caio Barbosa de Lima
Lucas

---

**Desenvolvido com ❤️ para a saúde e o meio ambiente**
