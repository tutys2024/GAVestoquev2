# 🚀 Implantação do Sistema de Estoque GAV com Firebase no GitHub Pages

Parabéns! Seu sistema de controle de estoque agora está integrado ao Firebase Realtime Database, permitindo leitura e escrita em tempo real. Este guia detalha os passos para implantar esta nova versão no GitHub Pages e configurar corretamente o Firebase.

## 1. Atualize as Regras de Segurança do Firebase

**IMPORTANTE:** Para que seu aplicativo possa ler e escrever dados no Firebase, você precisa ajustar as regras de segurança. Conforme discutimos, suas regras atuais expiram em 13 de agosto de 2025. Para fins de desenvolvimento e teste, você pode torná-las públicas. **Para produção, você DEVE implementar autenticação e regras mais restritivas.**

1.  Acesse o Console do Firebase: [https://console.firebase.google.com/](https://console.firebase.google.com/)
2.  Selecione seu projeto (`estoque1-c5809`).
3.  No menu lateral, vá em **Realtime Database**.
4.  Clique na aba **Regras**.
5.  Substitua o conteúdo atual pelo seguinte:

    ```json
    {
      "rules": {
        ".read": true,
        ".write": true
      }
    }
    ```

6.  Clique em **Publicar**.

## 2. Obtenha as Credenciais do Firebase

As credenciais do seu projeto Firebase são necessárias para que o aplicativo se conecte ao seu banco de dados. Eu já as inseri no arquivo `firebaseService.js` que está no ZIP, mas é bom saber onde encontrá-las para futuras referências ou depuração.

1.  No Console do Firebase, vá em **Configurações do Projeto** (ícone de engrenagem ao lado de "Visão geral do projeto").
2.  Clique na aba **Geral**.
3.  Role para baixo até a seção **Seus aplicativos**.
4.  Selecione o aplicativo web que você registrou (`Sistema de Estoque GAV`).
5.  Você verá um bloco de código `firebaseConfig`. As informações importantes são:
    *   `apiKey`
    *   `authDomain`
    *   `databaseURL`
    *   `projectId`
    *   `storageBucket`
    *   `messagingSenderId`
    *   `appId`

## 3. Implante o Aplicativo no GitHub Pages

Esta versão do aplicativo foi otimizada para ser implantada diretamente na raiz do seu repositório GitHub Pages. Isso significa que você não precisa de subpastas ou configurações complexas.

1.  **Baixe o arquivo ZIP anexo:** `estoque-gav-firebase.zip`.
2.  **Extraia o conteúdo** deste ZIP em uma pasta no seu computador. Você encontrará 7 arquivos (HTML, CSS, JS, manifest, ícones).
3.  **Vá para o seu repositório GitHub** (`https://github.com/tutys2024/GAVestoquev2` ou o repositório que você está usando).
4.  **Exclua todos os arquivos e pastas existentes** na raiz do seu repositório (exceto a pasta `.git` se você estiver usando Git localmente).
5.  **Faça o upload dos 7 arquivos extraídos** do ZIP diretamente para a raiz do seu repositório GitHub.
6.  **Faça um commit** das alterações.
7.  Aguarde alguns minutos (geralmente 2-5 minutos) para que o GitHub Pages atualize. Seu aplicativo estará acessível em `https://tutys2024.github.io/GAVestoquev2/` (ou a URL do seu repositório).

## 4. Teste o Sistema

Após a implantação, acesse a URL do seu GitHub Pages. Você deverá ver o sistema de estoque carregando os dados do Firebase. Tente:

*   **Adicionar um novo item**: Verifique se ele aparece no aplicativo e no seu Firebase Realtime Database.
*   **Editar um item**: Altere o estoque ou status e veja a atualização.
*   **Remover um item**: Confirme a remoção no aplicativo e no Firebase.

Se tiver qualquer problema, verifique o console do navegador (F12) em busca de erros e as regras do seu Firebase. Estou à disposição para ajudar!

