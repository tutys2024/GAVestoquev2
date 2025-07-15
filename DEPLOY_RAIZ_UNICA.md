# 🚀 Deploy Raiz Única - Sistema de Estoque GAV Resorts

## ✅ Estrutura Totalmente Plana

Todos os arquivos estão na **raiz única** do repositório, sem subdiretórios:

```
/ (raiz do repositório)
├── index.html                    # Página principal
├── index-D5dYHP65.js            # JavaScript compilado
├── index-n8Te3zif.css           # CSS compilado
├── manifest.json                # Configuração PWA
├── favicon.ico                  # Ícone do site
├── icon-192x192.png             # Ícone PWA 192x192
├── icon-512x512.png             # Ícone PWA 512x512
├── .nojekyll                    # Para GitHub Pages
├── .env.example                 # Configuração Firebase
├── eco-channel-*.json           # Chave Firebase
├── README.md                    # Documentação principal
├── DEPLOY_RAIZ_UNICA.md         # Este arquivo
└── [todos os arquivos .md]      # Documentação
```

## 🎯 Instruções de Deploy

### 1. Upload Simples
1. **Extrair** todos os arquivos do ZIP
2. **Selecionar TODOS** os arquivos (não a pasta)
3. **Arrastar e soltar** diretamente na raiz do repositório GitHub
4. **Commit** as alterações

### 2. Configuração GitHub Pages
1. Ir em **Settings > Pages**
2. Source: **Deploy from a branch**
3. Branch: **main** (ou master)
4. Folder: **/ (root)**
5. **Save**

### 3. Configuração Firebase
1. Renomear `.env.example` para `.env`
2. Configurar credenciais Firebase
3. Usar `eco-channel-*.json` como referência

## ✨ Vantagens da Raiz Única

- ✅ **Máxima compatibilidade** com GitHub Pages
- ✅ **Zero configuração** de caminhos
- ✅ **Deploy instantâneo** sem problemas de roteamento
- ✅ **Todos os arquivos acessíveis** diretamente
- ✅ **PWA funcionando** imediatamente

## 🔧 Arquivos Principais

- **index.html** - Página principal do sistema
- **index-D5dYHP65.js** - Todo o JavaScript compilado
- **index-n8Te3zif.css** - Todo o CSS compilado
- **manifest.json** - Configuração PWA
- **Ícones** - favicon.ico, icon-192x192.png, icon-512x512.png

## 📱 Sistema Completo

O sistema inclui todas as funcionalidades:
- Interface moderna e responsiva
- Sistema PWA com offline
- Integração Firebase em tempo real
- Controle de salas GAV Resorts
- Dashboard com estatísticas
- Sistema de pedidos e baixa

## 🌐 Acesso

Após deploy: `https://SEU_USUARIO.github.io/SEU_REPOSITORIO`

