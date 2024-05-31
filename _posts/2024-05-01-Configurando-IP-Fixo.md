---
layout: post
title: "Direto ao ponto - Configurando IP FIXO IPv4"
subtitle: "Demonstrando como configurar um IP fixo no seu servidor sem muitas dores de cabeça"
date: 2024-05-01 07:00:00 -0400
background: '/img/posts/bg/01.jpg'
---

Com o Gerenciador de Servidores aberto iremos seguir as etapas a baixo:

### Acessar as Configurações de Rede
No Server manager, vá até o Painel.
Clique em Local Server para exibir informações sobre o servidor.

![Server manager](/img/posts/img-01/1.PNG)

### Configurar o Endereço IP
Na seção Properties, localize a linha Ethernet (ou o nome do adaptador de rede que você deseja configurar) e clique no link ao lado dele. Isso abrirá a janela Network Connections.

![Ethernet](/img/posts/img-01/2.PNG)

Na janela Network Connections, clique com o botão direito no adaptador de rede IPv4 e selecione Properties.

![Properties Ethernet](/img/posts/img-01/3.PNG)

### Configurar o Protocolo TCP/IPv4
Na janela Propriedades da Conexão de Rede, selecione Protocolo IP Versão 4 (TCP/IPv4) e clique em Properties.

![Properties](/img/posts/img-01/4.PNG)

### Definir um Endereço IP Estático
Na janela Internet Protocol Version 4 Properties, selecione a opção Usar o seguinte endereço IP.
Preencha os campos:
Endereço IP: Insira o endereço IP estático que você deseja atribuir ao servidor.
Máscara de sub-rede: Insira a máscara de sub-rede correspondente à sua rede (por exemplo, `255.255.255.0`).
Gateway padrão: Insira o gateway padrão (Roteador) da sua rede.
Preencha os campos de DNS:
- Servidor DNS preferencial: Insira o endereço IP do servidor DNS principal.
- Servidor DNS alternativo: Insira o endereço IP do servidor DNS secundário, se houver.
Após o preenchimento das informações, aplique e confirme as alterações.

![Internet Protocol Version 4 Properties](/img/posts/img-01/5.PNG)

### Verificando se a configuração foi feita
Volte ao Server manager, vá até o Painel e em Ethernet vai está o novo endereço IPv4 configurado.

![Server manager](/img/posts/img-01/6.PNG)

Abre o `cmd` e faça testes de conexões utilizando o ping ou outra ferramenta de redes de sua preferência.