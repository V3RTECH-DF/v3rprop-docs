---
title: Política de Privacidade
parent: Legal
nav_order: 2
---

# Política de Privacidade

**V3RProp — Plugin de Propostas Comerciais para WordPress**

Versão 1.0 — Julho de 2026

---

{: .note }
> **Como ler este documento**
>
> O V3RProp é um plugin **auto-hospedado**: ele roda no WordPress do próprio
> usuário e os dados ficam no servidor dele. Por isso, este documento tem duas
> partes: **(A)** o que a V3RTECH faz com dados (praticamente nada) e **(B)**
> quais dados pessoais o plugin trata no ambiente do usuário — informação
> essencial para que o usuário cumpra a LGPD como **controlador** desses dados.

---

## Parte A — O papel da V3RTECH

**A.1.** A V3RTECH é a **fornecedora do software**. Ela desenvolve e distribui o plugin, mas **não hospeda, não acessa e não recebe** os dados de propostas, clientes ou aceites processados pelo V3RProp na instalação do usuário. Não há envio automático desses dados para a V3RTECH ("phone-home").

**A.2.** Eventuais dados de contato que o usuário forneça diretamente à V3RTECH (por exemplo, ao solicitar suporte ou adquirir o plugin) são tratados apenas para essa finalidade, conforme a LGPD (Lei nº 13.709/2018).

**A.3.** Encarregado de Proteção de Dados (DPO) da V3RTECH: [dpo@v3rtech.com.br](mailto:dpo@v3rtech.com.br).

---

## Parte B — Dados tratados pelo plugin (responsabilidade do usuário)

{: .important }
> **Quem é o controlador**
>
> Ao usar o V3RProp para tratar dados de seus clientes, **você (o usuário do
> plugin) é o controlador** desses dados pessoais, nos termos da LGPD. Cabe a
> você definir a base legal, informar os titulares e atender aos direitos deles.
> Esta seção descreve o que o plugin coleta, para você cumprir esse papel.

### B.1. Dados que o plugin armazena no seu servidor

| Dado | Origem | Onde é usado |
|---|---|---|
| Nome, e-mail, CNPJ, telefone, endereço e logo do cliente | Cadastro de clientes | Preenchimento e envio das propostas |
| Nome, cargo, e-mail e CPF/CNPJ do signatário | Aceite eletrônico | Registro da manifestação de vontade |
| Endereço IP, data/hora, agente de usuário (navegador) e hash de autenticidade | Aceite eletrônico | Evidência e auditoria do aceite |
| Endereço IP, agente de usuário e data/hora de visualização | Telemetria da proposta pública | Acompanhamento comercial |
| Nome, e-mail e conteúdo de comentários | Negociação na proposta pública | Comunicação com o cliente |

Todos esses dados ficam **no banco de dados do seu WordPress**, sob sua guarda.

### B.2. Bases legais (a definir pelo controlador)

O tratamento desses dados costuma apoiar-se em **execução de contrato ou procedimentos preliminares** (Art. 7º, V da LGPD) e em **legítimo interesse** (Art. 7º, IX) para segurança e evidência do aceite. Cabe a você confirmar a base adequada ao seu caso e informá-la aos titulares.

### B.3. Serviços de terceiros (quando você os configurar)

O plugin só contata serviços externos que **você** configurar:

| Serviço | Dados enviados | Quando |
|---|---|---|
| **Serviço de e-mail** do seu WordPress (SMTP/host) | E-mails transacionais (link da proposta, aceite, lembretes) | Ao notificar clientes |
| **Gotenberg** (geração de PDF), se configurado | Conteúdo da proposta para renderizar o PDF | Ao gerar PDF de alta fidelidade |
| **Ferramentas de automação** via API/webhook, se configuradas | Eventos e dados de proposta/cliente | Conforme sua automação |

A responsabilidade por contratar esses serviços e garantir conformidade (inclusive em eventuais transferências internacionais) é sua, na qualidade de controlador.

### B.4. Segredos e segurança

- Chave de API, senha do serviço de PDF e certificado ICP-Brasil (com senha) ficam no seu servidor e **nunca** são incluídos em exportações de dados do plugin.
- Recomenda-se restringir o acesso ao painel administrativo, manter o WordPress atualizado e usar HTTPS.

### B.5. Direitos dos titulares

Os titulares (seus clientes e signatários) têm os direitos previstos na LGPD — confirmação, acesso, correção, eliminação, portabilidade, entre outros. Como controlador, você os atende diretamente. O recurso **Importar/Exportar** ajuda a localizar e extrair dados quando necessário.

### B.6. Retenção e eliminação

Você define os prazos de retenção conforme sua necessidade e obrigações legais. A exclusão de clientes e propostas pelo painel remove os respectivos registros do seu banco de dados.

---

## Alterações nesta Política

Esta Política pode ser atualizada. A versão vigente estará sempre disponível em [docs-v3rprop.v3rtech.com.br/legal/privacidade](https://docs-v3rprop.v3rtech.com.br/legal/privacidade/).

---

## Contato

- **DPO da V3RTECH:** [dpo@v3rtech.com.br](mailto:dpo@v3rtech.com.br)
- **Suporte:** [suporte@v3rtech.com.br](mailto:suporte@v3rtech.com.br)
- **Comercial / Vendas:** [comercial@v3rtech.com.br](mailto:comercial@v3rtech.com.br)

---

*Versão 1.0 — Julho de 2026. Este documento descreve o comportamento do plugin quanto a dados pessoais e não substitui a assessoria jurídica que o controlador deve buscar para o seu caso concreto.*
