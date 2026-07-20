---
title: Precificação por Blocos
parent: Módulos
nav_order: 4
---

# Precificação por Blocos

A precificação do V3RProp é modular: em vez de um único "valor total", você combina **blocos de valor** que convivem na mesma proposta, cada um com o seu próprio subtotal. Isso deixa claro o que é implantação, o que é mensalidade e o que o cliente pode escolher.

![Bloco de precificação expandido no editor](/assets/screenshots/editor-precificacao.png)

## Os quatro tipos de bloco

| Tipo | Quando usar |
|---|---|
| **Lista de itens** | Vários componentes/serviços, cada um com valor de mercado, desconto e natureza (avulso, por hora, por evento ou "sob consulta"). Itens por hora/evento multiplicam pela quantidade. |
| **Implantação (valor único)** | Um único valor de setup/entrada — quando não faz sentido detalhar item a item. |
| **Serviço recorrente** | A mensalidade. Valor fixo ou variável por ciclo, periodicidade (mensal/trimestral/anual) e prazo (indeterminado ou nº fixo de ciclos). |
| **Opções / Pacotes** | Planos comparáveis lado a lado; o cliente escolhe um. Marque o **Recomendado** para guiar a decisão. |

## Recursos de cada bloco

- **Parcelamento** — habilite por bloco (ex.: parcelar só a implantação), com nº de parcelas e eventual acréscimo.
- **Importar do catálogo** — traga itens já cadastrados; o V3RProp cria o bloco certo conforme o tipo de cobrança de cada item.
- **Importar de Produtos e Serviços** — reaproveite o escopo já descrito.
- **Políticas comerciais** — aplique descontos e condições, no bloco ou em todos.

## Escolher quais cards aparecem no resumo

Na maioria dos casos o comportamento automático já é o certo, e você não precisa mexer. Mas quando quiser decidir na mão — por exemplo, mostrar um card de implantação **R$ 0,00** para deixar explícito ao cliente que a implantação é gratuita — o controle está no rodapé escuro de totais, na aba de Precificação, em **Cards no resumo da proposta**.

![Controle de exibição dos cards do resumo, no rodapé de totais da Precificação](/assets/screenshots/precificacao-cards-resumo.png)

Cada card tem três opções:

| Opção | O que faz |
|---|---|
| **Automático** (padrão) | O card aparece se tiver valor. É o comportamento descrito acima. |
| **Sempre exibir** | Força o card a aparecer, mesmo zerado. |
| **Nunca exibir** | Esconde o card, mesmo que tenha valor. |

Ao lado do nome de cada card, um selo mostra ao vivo como ele vai sair na proposta: **exibindo** ou **oculto**. Assim você confere sem precisar abrir a prévia.

{: .warning }
> **"Nunca exibir" some com o valor da vista do cliente.** Se você ocultar um card que tem valor, aquele número não aparece no resumo — embora os blocos de precificação acima continuem mostrando seus subtotais. Use com intenção.

## O importador inteligente

No nível da Precificação, o botão **Importar do catálogo** lê o tipo de cobrança de cada item selecionado e monta os blocos automaticamente:

- Item **pontual** → vira linha em um bloco **Lista de itens**.
- Item **recorrente** → vira um bloco **Serviço recorrente** com a periodicidade do item.
- Item **setup + recorrente** → cria um bloco de **Implantação** **e** um de **Serviço recorrente**.

{: .tip }
> **Menos digitação, menos erro**
>
> Cadastre bem o [catálogo](/modulos/catalogo/) uma vez e monte a precificação em segundos, sem redigitar valores nem esquecer a mensalidade.

## Como o cliente vê

Na proposta pública, cada bloco aparece com seu título e subtotal próprios. No rodapé, o V3RProp mostra o **investimento pontual** e o **recorrente (MRR)** separados — sem embolar os dois em um número só.

Esses dois cards do resumo aparecem **conforme a proposta**: se ela só tem mensalidade, o cliente vê apenas o card do recorrente; se só tem valores à vista, apenas o pontual; se tem os dois, os dois. Você não precisa configurar nada para isso — e uma proposta puramente recorrente não mostra mais um card de "R$ 0,00" ao lado da mensalidade.

![Seção de precificação na proposta pública](/assets/screenshots/publica-precificacao.png)

Quando você usa **Opções/Pacotes**, o cliente compara os planos lado a lado, com destaque para o Recomendado:

![Pacotes comparados lado a lado na proposta pública](/assets/screenshots/publica-opcoes.png)

{: .example }
> **Ancoragem com três pacotes**
>
> Ofereça três opções e destaque a do meio como "Recomendada". A opção mais cara valoriza a do meio; a mais barata dá um ponto de entrada. A maioria escolhe o meio — que costuma ser exatamente o que você quer vender.
