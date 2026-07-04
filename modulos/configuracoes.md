---
title: Configurações da Organização
parent: Módulos
nav_order: 7
---

# Configurações da Organização

Aqui ficam os dados globais da empresa que **emite** as propostas. Bem preenchidas, as Configurações alimentam toda proposta nova — você configura uma vez e colhe sempre.

![Tela de Configurações da Organização](/assets/screenshots/configuracoes.png)

## Identificação da organização

- **Nome, slogan e CNPJ** — a identidade da sua empresa.
- **Representante legal** — nome e CPF, usados nos documentos.
- **Logomarca** — selecionada pela Biblioteca de Mídia do WordPress, com pré-visualização.
- **E-mail corporativo** — para onde chegam as notificações (primeira visualização, comentários, aceite).

## Aparência padrão

- **Paleta de cores padrão** — cor primária, secundária e de destaque que as novas propostas herdam.
- **Validade padrão** — prazo em dias (padrão: 30).
- **Cabeçalho, rodapé, largura e ícone padrão** — os defaults visuais das propostas.

## Integrações

- **Chave de API externa** — gere uma chave para conectar o V3RProp a ferramentas externas (n8n, Make). Veja **[API REST e Automações](/modulos/api-rest/)**.
- **Webhook** — uma URL que recebe eventos (visualização, aceite) para automações.
- **Serviço de PDF (Gotenberg)** — opcional, para gerar PDFs de altíssima fidelidade. Informe URL, usuário e senha e use **Testar conexão**.

{: .important }
> **Trate a chave de API como uma senha**
>
> Quem tem a chave pode criar clientes e propostas via API. Não a compartilhe e gere uma nova se suspeitar de vazamento.

## Templates de e-mail

O V3RProp envia e-mails automáticos em cada etapa. Você pode personalizar o texto de cada um:

![Seção de templates de e-mail nas Configurações](/assets/screenshots/configuracoes-emails.png)

- Proposta publicada, confirmação de aceite, confirmação de ajuste/dúvida, confirmação de comentário, lembrete de expiração e aviso de expiração.
- Use variáveis dinâmicas (como o nome do cliente, o título e o link da proposta) para personalizar.
- Deixe um campo em branco para voltar ao texto padrão otimizado.

## Assinatura Digital ICP-Brasil

Para assinar os PDFs com o seu certificado A1:

- Envie o arquivo **`.pfx`/`.p12`** e informe a senha.
- O V3RProp avisa com **15, 5 e 1 dia** de antecedência quando o certificado estiver perto de vencer.
- Vencido o certificado, a assinatura volta automaticamente ao modelo eletrônico por IP/hash (que também tem validade legal).

{: .note }
> **Segurança dos segredos**
>
> A chave de API, a senha do serviço de PDF e o certificado (com a senha) **nunca** são incluídos em exportações de dados. Ver **[Importar e Exportar Dados](/modulos/importar-exportar/)**.
