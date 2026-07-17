# Guia de Publicação no GitHub Pages

## Passos para Publicar

### 1. Criar um repositório no GitHub

1. Acesse [github.com](https://github.com) e faça login
2. Clique no ícone **+** no canto superior direito
3. Selecione **New repository**
4. Nome do repositório: `nome-usuario.github.io` (substitua `nome-usuario` pelo seu usuário)
   - Ou use outro nome (Ex: `mostra-cientifica`)
5. Selecione **Public**
6. Clique **Create repository**

### 2. Preparar o Git Localmente

```bash
# Navegue até a pasta do projeto
cd "c:\Users\Bethania\Pictures\VIRUS"

# Inicialize o repositório git (se ainda não feito)
git init

# Configure seu usuário (primeira vez)
git config --global user.email "seu-email@example.com"
git config --global user.name "Seu Nome"

# Adicione todos os arquivos
git add .

# Crie o primeiro commit
git commit -m "Initial commit: projeto mostra científica"
```

### 3. Conectar ao Repositório do GitHub

```bash
# Adicione o repositório remoto (substitua com a URL do seu repositório)
git remote add origin https://github.com/seu-usuario/seu-repositorio.git

# Defina a branch principal como 'main'
git branch -M main

# Faça o push para o GitHub
git push -u origin main
```

### 4. Ativar GitHub Pages

1. No repositório do GitHub, vá para **Settings**
2. Procure por **Pages** na barra lateral esquerda
3. Em "Build and deployment":
   - Source: Selecione **Deploy from a branch**
   - Branch: Selecione **main** e pasta **/(root)**
4. Clique **Save**

### 5. Acessar o Site

Seu site será disponibilizado em:
- Se o repositório se chama `nome-usuario.github.io`: `https://nome-usuario.github.io`
- Se tem outro nome: `https://nome-usuario.github.io/seu-repositorio`

**Nota**: Pode levar alguns minutos para o site ficar disponível após o primeiro push.

## Arquivos Importantes

- **index.html** - Mapa interativo das constelações
- **dados.html** - Página de dados e curiosidades
- **README.md** - Documentação do projeto
- **.gitignore** - Arquivos a ignorar no Git

## Estrutura Recomendada para o Futuro

```
mostra-cientifica/
├── index.html
├── dados.html
├── README.md
├── .gitignore
├── css/ (opcional)
│   └── styles.css
├── js/ (opcional)
│   └── main.js
├── images/ (opcional)
│   └── constellation-images/
└── docs/ (opcional)
    └── documentacao.md
```

## Atualizações Futuras

Para fazer atualizações:

```bash
# Faça as alterações nos arquivos

# Adicione as mudanças
git add .

# Crie um commit
git commit -m "Descrição das mudanças"

# Faça o push
git push origin main
```

---

Qualquer dúvida, consulte a [documentação oficial do GitHub Pages](https://docs.github.com/en/pages)
