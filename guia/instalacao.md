---
title: Instalação e Primeiros Passos
parent: Guia de Uso
nav_order: 1
---

# Instalação e Primeiros Passos

O V3RProp é um plugin de WordPress. Você o instala no seu próprio site e trabalha inteiramente dentro do painel do WordPress (`wp-admin`) — nada de contas externas ou mensalidades de plataforma.

## Instalar o plugin

1. No painel do WordPress, acesse **Plugins → Adicionar novo → Enviar plugin**.
2. Selecione o arquivo `.zip` do V3RProp e clique em **Instalar agora**.
3. Depois de instalado, clique em **Ativar**.

Ao ativar, um novo item **V3RProp** aparece no menu lateral do WordPress, com o ícone de gráfico.

{: .note }
> **Requisitos**
>
> O V3RProp funciona em WordPress 5.8 ou superior, com PHP 7.4 ou superior. Para a geração de PDF de alta fidelidade e a assinatura ICP-Brasil, há configurações opcionais descritas em **[Configurações da Organização](/modulos/configuracoes/)**.

## Configurar a sua organização

Antes de criar a primeira proposta, preencha os dados da empresa que **emite** as propostas. Esses dados são reaproveitados em toda proposta e nos e-mails enviados ao cliente.

Acesse **V3RProp → Configurações** e preencha:

- **Identificação da organização** — nome, slogan, CNPJ, representante legal e logomarca (via Biblioteca de Mídia do WordPress).
- **E-mail corporativo** — para onde chegam as notificações (primeira visualização, comentários, aceite).
- **Paleta de cores padrão** — as cores que as novas propostas herdam.
- **Validade padrão** — por quantos dias a proposta fica válida (padrão: 30).

Veja o passo a passo completo em **[Configurações da Organização](/modulos/configuracoes/)**.

{: .tip }
> **Faça isso uma vez só**
>
> Bem configurada, a organização vira o "esqueleto" de todas as propostas: você abre uma proposta nova e já parte da sua identidade, cores e validade. Só ajusta o que for específico daquele cliente.

## O que preparar em seguida

Com a organização pronta, dois cadastros deixam o trabalho muito mais rápido:

- **[Clientes](/modulos/clientes/)** — cadastre quem recebe as propostas (razão social, contato, e-mail, logo). O e-mail do cliente é o que recebe notificações e serve ao aceite.
- **[Catálogo](/modulos/catalogo/)** — cadastre seus produtos e serviços com preço e tipo de cobrança. Depois é só importar para a precificação, sem redigitar.

Feito isso, você está pronto para **[criar sua primeira proposta](/guia/criar-proposta/)**.
