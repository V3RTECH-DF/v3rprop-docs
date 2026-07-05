---
title: Novidades
nav_order: 5
---

# Novidades

O que mudou no V3RProp, em linguagem simples. Para o histórico técnico completo, consulte o changelog no repositório do projeto.

## Dashboard e Propostas agora são telas separadas

O antigo painel único virou **dois itens de menu**: o **Dashboard**, só com os indicadores de vendas (e atalhos rápidos), e **Propostas**, com a lista completa para você buscar, filtrar e agir. Menos rolagem, cada coisa no seu lugar. Veja **[Dashboard](/modulos/dashboard/)** e **[Propostas](/modulos/propostas/)**.

## Configurações organizadas em abas

A tela de Configurações, que era longa, passou a ter **abas** — Organização, Parâmetros Comerciais, Layout Global, E-mails, Configurações Técnicas e Importação/Exportação — com um botão **Salvar** que grava tudo de uma vez. O backup/migração de dados agora fica na aba **Importação/Exportação**.

## Enviar feedback direto do painel

No cabeçalho de qualquer tela há agora dois botões: **Manual do Usuário** (abre este manual) e **Enviar Feedback**, para mandar sugestões, dúvidas ou relatos de bug à equipe V3RTECH sem sair do plugin — com um diagnóstico técnico automático que acelera o suporte, e sem expor seus dados sensíveis. Veja **[Ajuda e Feedback](/guia/ajuda-e-feedback/)**.

## Editor de propostas por blocos e dois modelos visuais

A maior novidade recente: a proposta deixou de ter seções fixas e passou a ser montada com **blocos livres** que você adiciona, reordena e combina como quiser — capa, texto, produtos e serviços, cronograma, precificação, razões, grids, citações e comparação de investimento.

Além disso, dois **modelos visuais**: o **Clássico** (sóbrio) e o **Moderno** (amplo, com imagens que ocupam a tela toda). Troca-se de modelo a qualquer momento, sem perder conteúdo.

## Precificação mais flexível

- **Serviços recorrentes** — cobre mensalidades com periodicidade e prazo, e o painel passa a mostrar a receita recorrente (MRR) separada do valor pontual.
- **Pacotes comparáveis** — apresente opções lado a lado com um "Recomendado".
- **Descontos e políticas em qualquer bloco** — aplique condições comerciais onde precisar.
- **Comparação de investimento** — mostre o valor de mercado riscado ao lado do seu, deixando a economia evidente.

## Catálogo mais completo

- **Foto, logomarca e link** por item, que viajam para a proposta.
- **Preços recorrentes e "setup + mensalidade"** direto no catálogo.
- **"Sob consulta"** — para itens sem preço fechado, que aparecem como "Sob consulta" sem quebrar a soma dos demais.
- **Importador inteligente** — selecione itens e o V3RProp monta os blocos de preço certos automaticamente.

## Capa com imagem de fundo

O bloco de capa (Hero) ganhou a opção de **usar a imagem como fundo da capa**, com sobreposição para manter o texto legível.

## Importar e exportar dados

Uma tela nova para **backup e migração**: exporte propostas, catálogo, clientes e configurações em um arquivo `.zip` e importe em outro servidor. Os segredos (chaves, senhas, certificado) nunca saem no arquivo.

## Acompanhamento e automação

- **Telemetria** de visualizações e aviso na primeira abertura.
- **Lembretes automáticos** de validade (5 dias e 1 dia antes) e expiração automática.
- **Versionamento** — renegocie publicando uma nova versão, com a antiga arquivada e redirecionamento do link.
- **API REST e webhooks** para integrar a n8n, Make e afins.
