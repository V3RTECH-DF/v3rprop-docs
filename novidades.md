---
title: Novidades
nav_order: 5
---

# Novidades

O que mudou no V3RProp, em linguagem simples — **da mais recente para a mais antiga**. Cada novidade traz a **versão** em que foi introduzida, para você saber o que é realmente novo.

{: .note }
> A versão instalada aparece no rodapé do painel e no cabeçalho do plugin (ex.: `v1.19.0`). Compare com a lista abaixo para ver o que você já tem.

---

## Proteção por senha reforçada
**v1.22.2 a v1.23.3 · julho de 2026**

O acesso a propostas protegidas por senha foi revisto de ponta a ponta, depois que identificamos que uma proposta protegida podia, em certas hospedagens, ser exibida sem a senha. O que mudou para você:

- A página de uma proposta com senha **não pode mais ser guardada em cache** por nenhuma camada do servidor — era essa a origem do problema.
- **Links antigos pararam de abrir direto.** Antes, o endereço enviado ao cliente carregava um código que dispensava a senha para sempre, inclusive para quem recebesse o link encaminhado. Esse mecanismo foi removido: agora o cliente informa a senha uma vez e segue com acesso liberado naquele navegador. **A senha continua a mesma e nada precisa ser reenviado.**
- **As senhas deixaram de ser guardadas de forma legível** no banco de dados do seu site. A conversão foi automática, sem nenhuma ação sua.
- Aceitar, recusar ou comentar uma proposta protegida agora também exige ter passado pela senha.

Veja **[Enviar a Proposta](/guia/enviar-proposta/)**.


## O contador regressivo agora desliga de verdade
**v1.22.1 · julho de 2026**

Desativar o contador regressivo de uma proposta não estava sendo salvo: ao reabrir, ele voltava ligado e continuava aparecendo para o cliente. Corrigido. Se você já tinha tentado desligá-lo em alguma proposta, **essa escolha foi recuperada** — não precisa refazer nada.


## Você escolhe quantos cards por linha
**v1.22.0 · julho de 2026**

Os blocos **Produtos e Serviços** e **Razões para a parceria** ganharam o seletor de **cards por linha** (2, 3 ou 4) que antes existia só no Grid de cards. O número é um limite, não uma obrigação: com menos cards do que colunas, eles crescem e preenchem a largura; sobrando um na última linha, ele também se estica. No celular, segue um por linha. Veja **[O Editor de Propostas](/modulos/editor/)**.


## Correções de exibição da proposta
**v1.21.1 · julho de 2026**

Duas correções discretas, mas que afetavam a proposta que vai ao cliente:

- A página deixou de **rolar levemente para os lados** no computador (um deslocamento de poucos pixels causado pela barra de rolagem).
- Uma proposta **publicada pela tela clássica do WordPress** deixou de sumir da lista de Propostas do V3RProp. Ela continuava acessível pelo link, mas não aparecia no painel; agora aparece normalmente, sem que você precise refazer nada.


## O resumo da proposta mostra só o que faz sentido
**v1.21.0 · julho de 2026**

Numa proposta que só tem mensalidade, o resumo mostrava um card **"Investimento pontual — R$ 0,00"** ao lado do valor recorrente. Isso acabou: agora cada card do resumo aparece conforme a proposta — só recorrente, só pontual, ou os dois. Não é preciso configurar nada.

Se quiser decidir na mão (por exemplo, exibir um **R$ 0,00** de propósito, para deixar claro que a implantação é gratuita), o novo controle **Cards no resumo da proposta**, no rodapé de totais da aba de Precificação, permite forçar **Sempre exibir** ou **Nunca exibir** cada card. Veja **[Precificação por Blocos](/modulos/precificacao/)**.


## Fim do selo "Recomendado" no resumo de valores
**v1.21.0 · julho de 2026**

O card de investimento pontual vinha com uma faixa **"RECOMENDADO"**, que aparecia sempre — inclusive sobre valores zerados. O selo foi removido, porque ele não fazia sentido ali: o investimento pontual e o recorrente **não são opções concorrentes** entre as quais o cliente escolhe; são duas partes do mesmo investimento (o que se paga uma vez e o que se paga por mês).

O **"Recomendado" continua existindo onde ele significa alguma coisa**: nos blocos de **Opções/Pacotes**, em que você marca qual plano quer destacar e o cliente de fato escolhe um.


## Cards ocupando a largura toda, em todos os blocos
**v1.21.0 e v1.21.2 · julho de 2026**

Os cards da proposta pública passaram a se distribuir pela largura inteira, qualquer que seja a quantidade — antes ficavam presos a colunas fixas, deixando espaço vazio à direita. Começou pelo resumo de investimento, pacotes e comparativo (v1.21.0) e se estendeu a **Produtos e Serviços**, **Razões para a parceria** e **Grid de cards** (v1.21.2). Um card sozinho agora ocupa a linha inteira.

## Status do certificado digital sempre correto
**v1.18.2 · julho de 2026**

O painel agora mostra com precisão a situação do seu certificado digital ICP-Brasil: enquanto válido, aparece **Certificado Ativo** (verde); assim que vence, passa a **Certificado Expirado** (vermelho, com a data em que venceu). Enquanto o certificado estiver vencido, as propostas aceitas continuam sendo assinadas eletronicamente por hash — nenhuma é assinada com um certificado fora da validade. Veja **[Configurações](/modulos/configuracoes/)**.

## Presets do catálogo à la carte
**v1.16.0 · julho de 2026**

Ao usar **Carregar Presets**, você agora escolhe exatamente o que importar — item a item, agrupado em Produtos & Serviços, Políticas e Conteúdos, com "Selecionar tudo" por grupo. O que já existe aparece marcado como "já no catálogo" e não é duplicado. E os presets passaram a incluir **conteúdos** prontos (institucional, razões, depoimento). Veja **[Catálogo](/modulos/catalogo/)**.

## Dashboard e Propostas em telas separadas; Configurações em abas
**v1.15.0 · julho de 2026**

O antigo painel único virou **dois itens de menu**: o **Dashboard**, só com os indicadores de vendas (e atalhos rápidos), e **Propostas**, com a lista completa. E a tela de **Configurações**, que era longa, passou a ter **abas** (Organização, Parâmetros Comerciais, Layout Global, E-mails, Configurações Técnicas e Importação/Exportação), com um botão **Salvar** que grava tudo de uma vez. Veja **[Dashboard](/modulos/dashboard/)** e **[Propostas](/modulos/propostas/)**.

## Feedback e manual no cabeçalho
**v1.14.0 · julho de 2026**

No cabeçalho de qualquer tela há dois botões: **Manual do Usuário** (abre este manual) e **Enviar Feedback**, para mandar sugestões, dúvidas ou relatos de bug à equipe V3RTECH sem sair do plugin — com um diagnóstico técnico automático que acelera o suporte, e sem expor seus dados sensíveis. Veja **[Ajuda e Feedback](/guia/ajuda-e-feedback/)**.

## Biblioteca de Conteúdos reaproveitáveis
**v1.13.0 · julho de 2026**

Nova aba **Conteúdos** no Catálogo: guarde textos que se repetem entre propostas (apresentação, razões, depoimentos) e insira em qualquer proposta com **"+ Da Biblioteca"** — ou salve um bloco existente com **"Salvar na biblioteca"**. Depoimentos ganharam **foto/avatar** de quem depõe. Veja **[Biblioteca de Conteúdos](/modulos/conteudos/)**.

## Bloco de Texto com título e aparência
**v1.12.0 · julho de 2026**

O bloco de Texto passou a aceitar um **título** e uma **aparência** — além do estilo padrão, os presets **Destaque**, **Nota** e **Atenção** (com fundo e barra lateral), mais ícone, imagem e ajuste de cor. Dá para diferenciar visualmente um trecho importante do resto. Veja **[Editor de Propostas e Blocos](/modulos/editor/)**.

---

## Recursos consolidados
*Presentes há mais tempo (versões v1.0 a v1.11) — a base do V3RProp.*

### Editor por blocos livres e dois modelos visuais
A proposta é montada com **blocos livres** que você adiciona, reordena e combina — capa, texto, produtos e serviços, cronograma, precificação, razões, grids, citações e comparação de investimento. E dois **modelos visuais**: **Clássico** (sóbrio) e **Moderno** (amplo, com imagens de tela cheia), trocáveis a qualquer momento sem perder conteúdo.

### Precificação flexível
- **Serviços recorrentes** — mensalidades com periodicidade e prazo; o painel mostra a receita recorrente (MRR) separada do valor pontual.
- **Pacotes comparáveis** — opções lado a lado com um "Recomendado".
- **Descontos e políticas em qualquer bloco.**
- **Comparação de investimento** — valor de mercado riscado ao lado do seu.

### Catálogo completo
Foto, logomarca e link por item; preços recorrentes e "setup + mensalidade"; **"Sob consulta"** para itens sem preço fechado; e um importador que monta os blocos de preço certos automaticamente.

### Capa com imagem de fundo
O bloco de capa (Hero) pode **usar a imagem como fundo da capa**, com sobreposição para manter o texto legível.

### Importar e exportar dados
**Backup e migração**: exporte propostas, catálogo, clientes e configurações num `.zip` e importe em outro servidor. Os segredos (chaves, senhas, certificado) nunca saem no arquivo. Hoje fica em **[Configurações → Importação/Exportação](/modulos/importar-exportar/)**.

### Acompanhamento e automação
Telemetria de visualizações com aviso na primeira abertura; lembretes automáticos de validade (5 e 1 dia antes) e expiração; versionamento (renegocie publicando uma nova versão, com a antiga arquivada); e **API REST + webhooks** para integrar a n8n, Make e afins.
