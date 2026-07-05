---
title: API REST e Automações
parent: Módulos
nav_order: 12
---

# API REST e Automações

O V3RProp oferece uma API REST para integrar suas propostas a ferramentas de automação como **n8n**, **Make** e afins — por exemplo, criar uma proposta automaticamente quando um lead avança no seu CRM.

{: .note }
> **Para quem é esta página**
>
> Esta é a única seção técnica do manual, voltada a quem monta automações. Se você só usa o painel, pode pular — nada aqui é obrigatório para o dia a dia.

## Autenticação

Gere uma **chave de API** em **[Configurações](/modulos/configuracoes/)**. Envie-a em cada requisição, no cabeçalho HTTP:

```
X-V3RProp-API-Key: SUA_CHAVE_DE_API
```

Ou como parâmetro de URL:

```
?api_key=SUA_CHAVE_DE_API
```

## Endpoints

| Método e rota | O que faz |
|---|---|
| `GET /wp-json/v3rprop/v1/external/clients` | Lista os clientes cadastrados. |
| `POST /wp-json/v3rprop/v1/external/clients` | Cria ou atualiza um cliente. |
| `GET /wp-json/v3rprop/v1/external/proposals` | Lista as propostas ativas. |
| `POST /wp-json/v3rprop/v1/external/proposals` | Cria ou atualiza uma proposta vinculada a um cliente. |

## Webhooks

Além de receber comandos, o V3RProp pode **avisar** sistemas externos quando algo acontece. Configure uma **URL de webhook** nas Configurações para receber eventos como **proposta visualizada** e **proposta aceita** — útil para disparar um fluxo no n8n assim que o cliente assina.

{: .tip }
> **Exemplo de automação**
>
> No n8n: ao ganhar um negócio no CRM, chame `POST /external/proposals` para gerar a proposta já preenchida; quando o webhook `proposal_accepted` disparar, atualize o CRM e notifique o time de entrega. Da oportunidade ao fechamento sem digitação manual.
