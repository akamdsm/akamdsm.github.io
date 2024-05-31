---
layout: post
title: "Direto ao ponto - Instalando o Active Directory"
subtitle: "Instalando o Active Directory no Windows Server 2016"
date: 2024-05-01 07:30:00 -0400
background: '/img/posts/bg/04.jpg'
---

No Server manager, observe o ícone de notificação com uma atenção amarela na parte superior direita da janela. Clique neste ícone para abrir a área de notificações.

![Notificação](/img/posts/img-04/1.PNG)

Na área de notificações, você verá uma mensagem indicando que o Serviço de Domínio Active Directory foi instalado. Clique na opção Promover este servidor a um controlador de domínio para iniciar o assistente de configuração.

### Configurando uma Nova Floresta
No assistente de configuração do Active Directory, selecione a opção Add a new forest. No campo de nome de domínio raiz, insira o nome do seu domínio, como por exemplo: `empresa.local`. Clique em Próximo para continuar.

![Nova floresta](/img/posts/img-04/2.PNG)

### Definindo Nível Funcional e Configurar DNS
Na próxima tela, defina o Nível funcional da floresta e o Nível funcional do domínio para Windows Server 2016. Certifique-se de que as opções Domain Name System (DNS) server e Global Catalog (GC) estejam marcadas. Em seguida, crie uma senha para o modo de restauração dos serviços de diretório (DSRM). Após configurar esses parâmetros, clique em Next.

![Nível funcional/ DNS](/img/posts/img-04/3.PNG)

Continue clicando em Próximo nas próximas telas, aceitando as configurações padrão fornecidas pelo assistente. Revise suas configurações na tela de resumo final e clique em Install para iniciar o processo de promoção.

![Nível funcional/ DNS](/img/posts/img-04/4.PNG)

Após a conclusão da instalação, o servidor será reiniciado automaticamente para aplicar as mudanças. Isso pode levar alguns minutos.

### Verificando a Configuração
Após o servidor reiniciar, faça login novamente. Abra o Server manager e vá até a seção AD DS para verificar o status.

![Verificando configuração](/img/posts/img-04/5.PNG)