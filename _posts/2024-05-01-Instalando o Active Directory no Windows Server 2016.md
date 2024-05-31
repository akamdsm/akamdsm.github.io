---
layout: post
title: "Direto ao ponto - Instalando o Active Directory"
subtitle: "Instalando o Active Directory no Windows Server 2016"
date: 2024-05-01 07:20:00 -0400
background: '/img/posts/bg/03.jpg'
---

Já no Server manager, localize e clique na opção Add roles and features. Isso iniciará o assistente que guiará o processo de instalação.

![Server manager](/img/posts/img-03/1.PNG)

### Selecionando o Tipo de Instalação
No assistente `Add roles and features`, você será apresentado a algumas opções de instalação. Selecione Role-based or feature-based installation e clique em Next para continuar.

![Add roles and features](/img/posts/img-03/2.PNG)

### Escolhendo o Servidor de Destino
Na etapa seguinte, você precisará selecionar o servidor onde deseja instalar o Active Directory. Seu servidor deve aparecer listado, então selecione-o e clique em Next.

![Servidor de destino](/img/posts/img-03/3.PNG)

### Selecionando a Função de Serviço de Domínio Active Directory
Agora, você verá uma lista de funções de servidor disponíveis. Role a lista e marque a caixa de seleção `Active Directory Domain Services`. Ao fazer isso, uma janela pop-up solicitará a adição de recursos necessários para esta função. Clique em Add Features para prosseguir.

![Selecionando a Função de Serviço de Domínio Active Directory](/img/posts/img-03/4.PNG)

### Prosseguindo com a Instalação
Depois de adicionar os recursos necessários, continue clicando em Próximo nas próximas telas, aceitando as configurações padrão. Na última tela de confirmação, revise suas seleções e clique em Install para iniciar a instalação.

![Prosseguindo com a Instalação](/img/posts/img-03/5.PNG)

### Finalizando a Instalação
Aguarde enquanto o processo de instalação é concluído. Isso pode levar alguns minutos. Após a instalação, será necessário promover o servidor a um controlador de domínio, mas isso será abordado em um artigo separado.