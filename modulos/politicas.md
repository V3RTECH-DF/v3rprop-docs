---
title: Políticas Comerciais
parent: Módulos
nav_order: 5
---

# Políticas Comerciais

As políticas comerciais são regras reutilizáveis que você aplica à precificação — descontos e condições — sem recalcular na mão a cada proposta. Elas ficam na aba **Políticas Comerciais**, dentro do Catálogo.

![Listagem de políticas comerciais](/assets/screenshots/politicas.png)

## Tipos de política

| Tipo | O que faz |
|---|---|
| **Desconto** | Aplica um abatimento percentual (ex.: `10%`) ou em valor (ex.: `R$ 500,00`) sobre o bloco de precificação. |
| **Combo** | Agrupa itens do catálogo como um conjunto. Disponível apenas nos blocos de lista de itens. |
| **Termos e condições** | Um texto de condições comerciais (pagamento, reajuste, prazos) que acompanha a proposta. |

## Cadastrar uma política

Clique em **Nova Política** e informe:

- **Nome** — ex.: "Desconto de Lançamento".
- **Tipo** — desconto, combo ou termos.
- **Valor** — o percentual ou valor (para descontos) ou os itens (para combo).
- **Descrição / regra** — a condição em si (no caso de termos, o texto que o cliente lê).

## Aplicar na proposta

Ao montar a [Precificação](/modulos/precificacao/), use **Aplicar Política** no bloco desejado e escolha o escopo:

- **Somente este bloco** — o desconto vale só ali.
- **Todos os blocos de itens** — o desconto se espalha pelos blocos aplicáveis.

O V3RProp mantém o **valor de referência** (de mercado) e mostra o abatimento de forma transparente na proposta pública — o cliente enxerga quanto está economizando.

{: .warning }
> **Desconto tem custo**
>
> Desconto não é a única resposta a "está caro". Muitas vezes o certo é ajustar escopo, não preço. Use políticas de desconto com critério — veja **[Respondendo às Dúvidas do Cliente](/vendas/respondendo-duvidas/)**.
