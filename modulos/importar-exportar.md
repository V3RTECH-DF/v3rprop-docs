---
title: Importar e Exportar Dados
parent: Módulos
nav_order: 9
---

# Importar e Exportar Dados

Esta tela permite fazer **backup** dos seus dados e **migrar** o V3RProp entre servidores (por exemplo, do ambiente de testes para produção, ou para um novo site).

![Tela de importar e exportar dados](/assets/screenshots/importar-exportar.png)

## Exportar

Escolha as categorias que quer levar e clique em **Exportar**:

- **Propostas**
- **Catálogo** (produtos e políticas)
- **Clientes**
- **Configurações da Organização**

O V3RProp gera um arquivo **`.zip`** com os dados (em JSON) e as mídias reais (fotos, logos). O download começa automaticamente.

{: .important }
> **O que nunca é exportado**
>
> Por segurança, ficam de fora do arquivo: a **chave de API externa**, a **senha do serviço de PDF**, o **certificado ICP-Brasil e a sua senha**, e os **PDFs de propostas aceitas** (regerados sob demanda no destino). Você reconfigura esses segredos no servidor de destino.

## Importar

Selecione um arquivo `.zip` exportado e clique em **Importar**.

{: .warning }
> **A importação só cria — nunca sobrescreve**
>
> Importar **cria registros novos** a partir do arquivo; não faz merge nem substitui o que já existe, e não pode ser desfeito automaticamente. Se importar duas vezes, você terá dados duplicados. Importe em um ambiente limpo quando o objetivo for migração.

Ao concluir, o V3RProp mostra um resumo do que foi criado (quantos clientes, itens de catálogo, políticas e propostas). Os vínculos entre entidades — proposta→cliente, produto→catálogo — são remapeados automaticamente.
