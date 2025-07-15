# 🚀 Deploy no GitHub Pages - Sistema de Estoque GAV Resorts

## Instruções Rápidas para Deploy

### 1. Preparação do Repositório
1. Crie um novo repositório no GitHub
2. Faça upload de TODOS os arquivos desta pasta para a **raiz** do repositório
3. Certifique-se de que o arquivo `.nojekyll` está presente na raiz

### 2. Configuração do GitHub Pages
1. Vá para Settings > Pages no seu repositório
2. Em "Source", selecione "Deploy from a branch"
3. Escolha a branch "main" (ou "master")
4. Selecione "/ (root)" como pasta
5. Clique em "Save"

### 3. Configuração do Firebase
1. Renomeie `.env.example` para `.env`
2. Configure suas credenciais do Firebase no arquivo `.env`
3. Use o arquivo `eco-channel-465718-n3-e5a66fce092b.json` como referência para configuração

### 4. Estrutura de Arquivos na Raiz
```
/
├── index.html              # Página principal
├── manifest.json           # Configuração PWA
├── favicon.ico             # Ícone do site
├── icon-192x192.png        # Ícone PWA 192x192
├── icon-512x512.png        # Ícone PWA 512x512
├── .nojekyll               # Arquivo para GitHub Pages
├── .env.example            # Exemplo de configuração
├── README.md               # Documentação principal
├── DEPLOY_GITHUB_PAGES.md  # Este arquivo
├── assets/                 # Arquivos JavaScript e CSS
│   ├── index-D5dYHP65.js   # JavaScript compilado
│   └── index-n8Te3zif.css  # CSS compilado
├── docs/                   # Documentação completa
└── eco-channel-*.json      # Chave do Firebase
```

### 5. Verificação
- Após o deploy, acesse: `https://SEU_USUARIO.github.io/SEU_REPOSITORIO`
- O sistema deve carregar automaticamente
- Verifique se o PWA está funcionando (ícone de instalação no navegador)

### 6. Funcionalidades Incluídas
✅ Sistema PWA completo  
✅ Interface responsiva  
✅ Integração Firebase  
✅ Controle de estoque em tempo real  
✅ Sistema de salas GAV Resorts  
✅ Dashboard com estatísticas  
✅ Funcionalidades offline  

### 7. Suporte
Consulte a pasta `docs/` para documentação detalhada e guias de configuração.

