---
layout: post
title: "Direto ao ponto - Configurando Hostname"
subtitle: "Demonstrando como configurar um hostname no seu servidor sem muitas dores de cabeça"
date: 2024-05-01 07:10:00 -0400
background: '/img/posts/bg/02.jpg'
---

Com o Server manager aberto iremos seguir as etapas a baixo:

### Acessando as propriedades do sistema
No Server manager, vá até o Local Server.
No Local Server, clique no link ao lado de Computer name.

![Local Server](/img/posts/img-02/1.PNG)

### Abrindo as Configurações de Nome do Computador
Na janela System Properties, vá para a aba Computer Name.
Clique no botão Change para abrir a janela Computer Name/Domain Changes.

![Local Server](/img/posts/img-02/2.PNG)

### Alterando o Nome do Computador
Na janela Computer Name/Domain Changes, no campo Computer name, digite o novo hostname do servidor.
Clique em OK para confirmar a mudança do nome do computador.

![Local Server](/img/posts/img-02/3.PNG)

Uma janela será exibida informando que é necessário reiniciar o computador para aplicar as alterações. Clique em OK.
Na janela System Properties, clique em Close.
Uma mensagem será exibida perguntando se você deseja reiniciar o computador agora. Clique em Restart Now para reiniciar o servidor imediatamente.

![Local Server](/img/posts/img-02/4.PNG)

### Verificando a Alteração
Após a reinicialização, faça login no servidor.
Abra o Server manager e verifique o painel Properties para confirmar que o hostname foi alterado corretamente.
É possível verificar via Prompt de Comando e digitando o comando `hostname` para verificar o novo nome do computador.