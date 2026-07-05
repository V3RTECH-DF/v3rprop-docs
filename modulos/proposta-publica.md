---
title: A Proposta Pública e o Aceite
parent: Módulos
nav_order: 10
---

# A Proposta Pública e o Aceite

Esta é a tela que o **cliente** vê — a razão de existir do V3RProp. É uma página standalone, aberta por um link único, sem o cabeçalho ou o menu do seu site, focada 100% na decisão.

![Proposta pública completa, como o cliente vê](/assets/screenshots/publica-completa.png)

## A experiência do cliente

- **Capa de impacto** — a chamada e o título vindos do bloco Hero, com a logo do cliente e as cores da proposta.
- **Carregamento rápido** — página leve e responsiva, boa no celular e no desktop.
- **Contador de escassez** (se ativado) — mostra quanto tempo resta de validade.

![Topo da proposta pública, com a capa](/assets/screenshots/publica-capa.png)

## Negociar sem sair da proposta

No rodapé, o cliente pode deixar **comentários e dúvidas**. Cada um gera uma notificação para o seu e-mail e uma confirmação para o cliente. Comentar **não invalida** a proposta — ela segue ativa. Você responde pela aba [Comentários](/modulos/editor/) do editor.

![Seção de comentários na proposta pública](/assets/screenshots/publica-comentarios.png)

## Aceite eletrônico

Quando o cliente decide fechar, ele preenche o formulário de aceite: **nome, cargo, e-mail e CPF/CNPJ**, e confirma.

![Formulário de aceite eletrônico na proposta pública](/assets/screenshots/publica-aceite.png)

Ao confirmar, o V3RProp:

1. Registra **data/hora, IP, navegador** e um **hash de autenticidade** — uma trilha auditável com validade jurídica (MP 2.200-2/2001).
2. Gera um **PDF assinado** da proposta.
3. Envia o PDF por e-mail para o cliente e para você.
4. Muda o status para **Aceita**.

Se você configurou a **[assinatura ICP-Brasil](/modulos/configuracoes/)**, o PDF é assinado com o seu certificado A1.

## Solicitar ajustes ou recusar

Se o cliente precisar de mudanças ou quiser declinar, ele usa o **formulário de recusa**, informando os motivos. A proposta vira **Recusada** e você recebe os motivos por e-mail — insumo valioso para a próxima versão ou para aprender. Ver **[Entendendo o Não](/vendas/entendendo-o-nao/)**.

## Auditoria: a aba Histórico

Do seu lado, tudo fica registrado na aba **Histórico** do editor:

![Certificado de aceite e logs de visualização na aba Histórico](/assets/screenshots/editor-historico.png)

- **Certificado de Aceite Digital** — signatário, e-mail, documento, data/hora, IP e navegador.
- **Histórico de versões** — as versões anteriores arquivadas (Substituídas).
- **Log de visualizações** — cada abertura da proposta pelo cliente, com IP e dispositivo.

## Versionamento

Renegociou? Ao **Publicar como Nova Versão**, a versão atual é arquivada como **Substituída** e o link público passa a exibir a nova. Se o cliente abrir um link antigo, é avisado de que há uma versão mais recente, com um atalho para ela.
