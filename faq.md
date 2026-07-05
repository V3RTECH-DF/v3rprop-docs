---
title: Perguntas Frequentes
nav_order: 6
---

# Perguntas Frequentes

## Começando

<details markdown="1">
<summary>Onde encontro o V3RProp depois de instalar?</summary>

No menu lateral do painel do WordPress, procure o item **V3RProp** (ícone de gráfico).
Ele reúne Dashboard, Propostas, Catálogo, Clientes, Configurações e Documentação
(o backup/migração fica dentro de Configurações). Veja **[Conhecendo o Painel](/guia/navegacao/)**.
</details>

<details markdown="1">
<summary>Qual é a primeira coisa que devo configurar?</summary>

As **Configurações da Organização** (V3RProp → Configurações): nome, logo,
e-mail, cores e validade padrão. Elas alimentam todas as propostas que você
criar depois. Em seguida, cadastre alguns **clientes** e itens do **catálogo**
para agilizar. Passo a passo em **[Instalação e Primeiros Passos](/guia/instalacao/)**.
</details>

<details markdown="1">
<summary>Preciso de uma conta na nuvem ou pagar mensalidade de plataforma?</summary>

Não. O V3RProp é um plugin que roda no **seu próprio WordPress**. Os dados ficam
no seu servidor e você trabalha inteiramente dentro do `wp-admin`.
</details>

<details markdown="1">
<summary>Como envio uma sugestão ou reporto um problema?</summary>

Use o botão **Enviar Feedback** no canto superior direito de qualquer tela do
V3RProp. Escolha o tipo (Sugestão, Dúvida ou Bug), escreva sua mensagem e envie —
um diagnóstico técnico (sem dados pessoais) vai junto para acelerar o suporte, e
você recebe uma cópia por e-mail. Detalhes em **[Ajuda e Feedback](/guia/ajuda-e-feedback/)**.
</details>

## Criando e enviando propostas

<details markdown="1">
<summary>Meu cliente não consegue abrir a proposta. Por quê?</summary>

Duas causas comuns: a proposta ainda está em **Rascunho** (publique-a com
**Salvar e publicar**) ou ela tem uma **senha de acesso** definida na aba
Identidade (informe a senha ao cliente por um canal separado).
</details>

<details markdown="1">
<summary>Qual a diferença entre os modelos Clássico e Moderno?</summary>

O **Clássico** é sóbrio, com cards de borda e largura contida — bom para
públicos formais. O **Moderno** é amplo, com imagens que ocupam a tela toda e
tipografia maior — mais impactante. Você troca de um para o outro a qualquer
momento, sem perder conteúdo. Ver **[Editor de Propostas e Blocos](/modulos/editor/)**.
</details>

<details markdown="1">
<summary>Como coloco uma mensalidade (valor recorrente) na proposta?</summary>

Na Precificação, adicione um bloco **Serviço recorrente** e informe o valor por
ciclo, a periodicidade e o prazo. Ou cadastre o item como **recorrente** no
[catálogo](/modulos/catalogo/) e importe — o bloco é criado automaticamente.
O painel passa a mostrar a receita recorrente (MRR) separada do valor pontual.
</details>

<details markdown="1">
<summary>Tenho um serviço sem preço fechado. Como apresentar?</summary>

Cadastre o item no catálogo com o tipo de cobrança **Sob consulta**. Ele aparece
na proposta como "Sob consulta" no lugar do preço e **não entra na soma** dos
demais itens. Você negocia o valor à parte.
</details>

<details markdown="1">
<summary>Como reaproveito uma proposta que deu certo?</summary>

Na tela **Propostas**, use a ação **Duplicar** na linha da proposta. Ela cria
uma cópia que você ajusta para o novo cliente — a forma mais rápida de manter o
padrão de qualidade.
</details>

## Aceite e validade jurídica

<details markdown="1">
<summary>O aceite eletrônico tem validade jurídica?</summary>

Sim. Ao aceitar, o V3RProp registra nome, e-mail, CPF/CNPJ, data/hora, IP,
navegador e um **hash de autenticidade** — uma trilha auditável amparada pela
MP 2.200-2/2001. Um PDF assinado é gerado e enviado às duas partes.
Ver **[A Proposta Pública e o Aceite](/modulos/proposta-publica/)**.
</details>

<details markdown="1">
<summary>Preciso de certificado ICP-Brasil?</summary>

Não é obrigatório. O aceite eletrônico por IP/hash já tem validade legal. Se você
quiser assinar os PDFs com um certificado **A1**, configure-o em Configurações —
o V3RProp ainda avisa quando ele estiver perto de vencer.
</details>

<details markdown="1">
<summary>Comentar na proposta cancela ou invalida ela?</summary>

Não. Os comentários e dúvidas do cliente **não invalidam** a proposta — ela segue
ativa. Só o formulário de recusa muda o status para Recusada.
</details>

## Acompanhamento

<details markdown="1">
<summary>Como sei se o cliente abriu a proposta?</summary>

O V3RProp registra cada visualização (data, IP, dispositivo) e te avisa por
e-mail na **primeira** abertura. O histórico completo fica na aba **Histórico**
do editor.
</details>

<details markdown="1">
<summary>Preciso ficar cobrando o cliente antes de a proposta vencer?</summary>

Não precisa lembrar disso: o V3RProp envia lembretes automáticos ao cliente
faltando **5 dias** e **1 dia** para a validade, e marca como **Expirada** se
ninguém aceitar. Você recebe cópia dessas mensagens.
</details>

<details markdown="1">
<summary>O cliente pediu mudanças. Como renegocio sem perder o histórico?</summary>

Edite a proposta e use **Publicar como Nova Versão**. A versão anterior é
arquivada como **Substituída** e o link público passa a mostrar a nova. Quem
abrir um link antigo é avisado de que existe uma versão atualizada.
</details>

## Dados e migração

<details markdown="1">
<summary>Como levo meus dados para outro servidor?</summary>

Use **Importar/Exportar**: gere um `.zip` com propostas, catálogo, clientes e
configurações e importe no servidor de destino. A importação **cria** registros
novos (não sobrescreve). Segredos como chaves e certificado não vão no arquivo —
reconfigure-os no destino. Ver **[Importar e Exportar Dados](/modulos/importar-exportar/)**.
</details>

<details markdown="1">
<summary>O PDF não está sendo gerado com a qualidade que espero.</summary>

O V3RProp gera PDF nativamente. Para fidelidade máxima ao layout web, configure o
serviço opcional **Gotenberg** em Configurações (URL, usuário, senha) e use
**Testar conexão**.
</details>
