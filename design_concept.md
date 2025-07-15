# Conceito de Design e UI/UX para o Sistema de Controle de Estoque GAV

Com base nos requisitos do usuário e na pesquisa de referências de design, o objetivo é criar um PWA de controle de estoque que seja:

*   **Completo e Funcional**: Atendendo a todas as necessidades de gerenciamento de estoque, incluindo CRUD, pedidos e baixas.
*   **Intuitivo e Fácil de Usar**: Com uma curva de aprendizado mínima para novos usuários.
*   **Harmonioso e Moderno**: Com um design limpo, visualmente atraente e responsivo.
*   **Rastreável**: Com controle de alterações por sala e usuário.

## 1. Elementos Chave de UI/UX

### 1.1. Fluxo de Seleção de Sala/Usuário (Prioritário)

*   **Tela Inicial**: Antes de acessar o dashboard principal, o usuário será solicitado a selecionar a `Sala` e, opcionalmente, inserir seu `Nome` ou `ID`.
*   **Componente de Seleção**: Utilizar um dropdown claro e com opções pré-definidas para as salas (conforme a imagem fornecida: Sala Gramado, Sala Luguito, Sala Hortênsias, Sala Rua Coberta).
*   **Campo de Usuário**: Um campo de texto simples para o nome/ID do usuário. Este campo pode ser opcional ou ter uma validação básica.
*   **Persistência**: A seleção da sala e o nome do usuário serão armazenados localmente (ex: Local Storage) para evitar que o usuário precise selecionar a cada acesso, mas com a opção de alterar.

### 1.2. Dashboard Principal

*   **Visão Geral**: Um dashboard claro e conciso, exibindo métricas importantes como:
    *   Total de Itens em Estoque
    *   Itens com Estoque Baixo (Alertas)
    *   Itens em Pedido/Aguardando Baixa
    *   Itens OK
*   **Cards Informativos**: Utilizar cards visuais para cada métrica, com ícones e cores que transmitam o status rapidamente.
*   **Barra de Pesquisa/Filtros**: Uma barra de pesquisa proeminente para encontrar itens rapidamente, e filtros para categorias, status, etc.

### 1.3. Lista de Itens de Estoque

*   **Visualização Clara**: Uma lista ou tabela de itens com informações essenciais visíveis de imediato: Nome do Item, Estoque Real, Depósito (se aplicável), Status (OK, Alerta, Pedido).
*   **Ações Rápidas**: Botões de ação intuitivos para cada item (ex: `Realizar Pedido`, `Dar Baixa`, `Editar`, `Detalhes`).
*   **Indicadores Visuais**: Utilizar cores ou ícones para indicar o status do estoque (verde para OK, amarelo para Alerta, vermelho para Estoque Negativo/Pedido).

### 1.4. Formulários de Alteração (Adicionar/Editar/Pedido/Baixa)

*   **Modais/Páginas Dedicadas**: Utilizar modais ou páginas separadas para formulários de adição, edição, realização de pedidos e baixa de estoque.
*   **Campos Claros**: Campos de entrada bem rotulados e com validação.
*   **Registro de Transação**: Para pedidos e baixas, incluir campos para `Quantidade`, `Observações` e registrar automaticamente a `Sala` e o `Usuário` que realizou a ação, além do `Timestamp`.

## 2. Estilo Visual e Harmonia

*   **Paleta de Cores**: Cores claras e modernas, com tons de azul/verde para elementos positivos/OK, amarelo para atenção e vermelho para alertas/problemas. Neutros para o fundo e texto.
*   **Tipografia**: Fontes limpas e legíveis, como `Inter` ou `Roboto`, para garantir boa leitura em diferentes dispositivos.
*   **Ícones**: Utilizar uma biblioteca de ícones consistente (ex: Material Design Icons ou Font Awesome) para representar ações e status.
*   **Responsividade**: O design será adaptável a diferentes tamanhos de tela (desktop, tablet, mobile) para garantir uma experiência de usuário consistente em qualquer dispositivo.
*   **Componentes**: Reutilizar componentes UI (cards, botões, inputs, dropdowns) para manter a consistência visual e acelerar o desenvolvimento.

## 3. Considerações Técnicas para UI/UX

*   **Framework UI**: Continuar utilizando Tailwind CSS para estilização rápida e responsiva.
*   **Componentes Reutilizáveis**: Criar componentes React bem definidos para cada parte da UI (Header, Sidebar, ItemCard, Forms).
*   **Gerenciamento de Estado**: Utilizar `useState` e `useEffect` do React para gerenciar o estado da aplicação, incluindo os dados do Firebase e a seleção de sala/usuário.

Este conceito de design servirá como base para a implementação do PWA, garantindo que ele atenda aos requisitos funcionais e de usabilidade.

