# Sistema de Controle de Estoque - GAV Resorts

Um Progressive Web App (PWA) moderno para controle de estoque integrado com Google Sheets, desenvolvido especificamente para GAV Resorts.

## 🚀 Características

- **PWA Completo**: Funciona offline, instalável no dispositivo
- **Integração Google Sheets**: Sincronização automática com planilhas
- **Interface Responsiva**: Otimizado para desktop e mobile
- **Dashboard Interativo**: Visualização de estatísticas em tempo real
- **Sistema de Alertas**: Notificações para itens com estoque baixo
- **Busca Avançada**: Filtros e pesquisa em tempo real
- **Gestão de Categorias**: Organização por categorias (BAR, KIDS, etc.)

## 🛠️ Tecnologias Utilizadas

- **React 19** - Framework frontend
- **Vite** - Build tool e dev server
- **Tailwind CSS** - Framework CSS
- **shadcn/ui** - Componentes UI
- **Lucide React** - Ícones
- **Recharts** - Gráficos e visualizações
- **Google Sheets API** - Integração com planilhas

## 📦 Instalação

1. **Clone o repositório ou extraia o arquivo ZIP**
   ```bash
   cd estoque-pwa-gav-resorts
   ```

2. **Instale as dependências**
   ```bash
   pnpm install
   # ou
   npm install
   # ou
   yarn install
   ```

3. **Configure as credenciais do Google Sheets**
   - Coloque o arquivo de credenciais JSON na pasta `src/data/`
   - Atualize o caminho no arquivo `src/services/googleSheetsService.js`

4. **Inicie o servidor de desenvolvimento**
   ```bash
   pnpm run dev
   # ou
   npm run dev
   ```

5. **Acesse a aplicação**
   - Abra [http://localhost:5173](http://localhost:5173) no navegador

## 🏗️ Build para Produção

```bash
pnpm run build
# ou
npm run build
```

Os arquivos otimizados serão gerados na pasta `dist/`.

## 📱 Instalação como PWA

1. Acesse a aplicação no navegador
2. Clique no ícone de "Instalar" na barra de endereços
3. Ou use o menu do navegador > "Instalar aplicativo"

## 🗂️ Estrutura do Projeto

```
estoque-pwa-gav-resorts/
├── public/
│   ├── manifest.json          # Configuração PWA
│   ├── sw.js                  # Service Worker
│   └── images/                # Imagens públicas
├── src/
│   ├── components/            # Componentes React
│   │   ├── ui/               # Componentes shadcn/ui
│   │   ├── AddItemForm.jsx   # Formulário adicionar item
│   │   ├── EstoqueDashboard.jsx # Dashboard principal
│   │   ├── EstoqueList.jsx   # Lista de itens
│   │   └── PWANotifications.jsx # Notificações PWA
│   ├── hooks/                # Custom hooks
│   │   ├── useEstoque.js     # Hook principal do estoque
│   │   └── usePWA.js         # Hook para funcionalidades PWA
│   ├── services/             # Serviços externos
│   │   └── googleSheetsService.js # Integração Google Sheets
│   ├── data/                 # Dados e configurações
│   ├── assets/               # Assets estáticos
│   ├── App.jsx               # Componente principal
│   ├── App.css               # Estilos principais
│   └── main.jsx              # Ponto de entrada
├── package.json              # Dependências e scripts
└── README.md                 # Este arquivo
```

## 🔧 Configuração

### Google Sheets API

1. Crie um projeto no [Google Cloud Console](https://console.cloud.google.com/)
2. Ative a Google Sheets API
3. Crie uma conta de serviço e baixe o arquivo JSON
4. Coloque o arquivo na pasta `src/data/`
5. Compartilhe sua planilha com o email da conta de serviço

### Variáveis de Ambiente

Crie um arquivo `.env` na raiz do projeto:

```env
VITE_GOOGLE_SHEETS_ID=sua_planilha_id
VITE_GOOGLE_SHEETS_RANGE=Sheet1!A:Z
```

## 📊 Funcionalidades

### Dashboard
- Visão geral do estoque
- Estatísticas em tempo real
- Gráficos de categorias
- Alertas de estoque baixo

### Gestão de Itens
- Adicionar novos itens
- Editar itens existentes
- Busca e filtros
- Categorização automática

### PWA Features
- Funciona offline
- Instalável no dispositivo
- Notificações push
- Sincronização automática

## 🤝 Contribuição

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📝 Licença

Este projeto é propriedade da GAV Resorts. Todos os direitos reservados.

## 📞 Suporte

Para suporte técnico, entre em contato com a equipe de TI da GAV Resorts.

---

**GAV Resorts** - Sistema de Controle de Estoque v1.0

