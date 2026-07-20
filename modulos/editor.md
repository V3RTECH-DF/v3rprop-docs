---
title: Editor de Propostas e Blocos
parent: Módulos
nav_order: 3
---

# Editor de Propostas e Blocos

O editor é onde a proposta ganha forma. Ele se divide em abas no menu lateral: **Identidade & Layout**, **Conteúdo (Blocos)** e — depois de a proposta existir — **Comentários** e **Histórico**.

## Aba Identidade & Layout

Define a aparência e os dados gerais da proposta.

![Aba de identidade e layout do editor](/assets/screenshots/editor-identidade.png)

- **Cliente** — vincula um cliente cadastrado (traz nome, e-mail e logo) ou usa dados avulsos.
- **Título interno** — nome de referência no painel.
- **Modelo de apresentação** — **Clássico** ou **Moderno** (veja abaixo).
- **Templates visuais** — conjuntos prontos de cores e fonte.
- **Paleta de cores** — cor primária, secundária e de destaque, ajustáveis individualmente.
- **Validade e contador de escassez** — prazo da proposta e o timer regressivo opcional.
- **Fonte, largura e ícone padrão** — refinamentos de tipografia e layout.
- **Cabeçalho e rodapé** — tamanho da logo e cores das barras.
- **Senha de acesso** — protege a proposta, se preenchida.

### Clássico ou Moderno?

| Modelo | Cara |
|---|---|
| **Clássico** | Sóbrio e objetivo, com cards de borda e largura contida. Ótimo para públicos mais formais. |
| **Moderno** | Amplo, com imagens que ocupam a tela toda (full-bleed), tipografia maior e cards com sombra. Mais impactante. |

Você troca de modelo a qualquer momento, sem perder conteúdo — o mesmo material é reestilizado.

## Aba Conteúdo (Blocos)

Aqui você empilha os **blocos** que formam o corpo da proposta. Cada bloco é adicionável, reordenável (setas ↑↓) e removível.

![Canvas de blocos livres do editor](/assets/screenshots/editor-blocos.png)

### Os tipos de bloco

| Bloco | Para que serve |
|---|---|
| **Capa (Hero)** | O primeiro bloco Hero alimenta a capa: chamada (kicker), título forte, subtítulo e imagem de fundo opcional. |
| **Texto** | Parágrafos livres, escritos no **editor de texto formatado** (veja abaixo). Aceita um **título opcional** e uma **aparência**: além do estilo Padrão, os presets **Destaque**, **Nota** e **Atenção** (com fundo e barra lateral), mais **ícone**, **imagem** e ajuste fino de cor — para diferenciar um bloco de texto dos demais. |
| **Produtos e Serviços** | Cards de escopo, cada um com título, **descrição**, entregáveis, foto, logomarca e link. Importável do catálogo. Você escolhe quantos **cards por linha** (2, 3 ou 4). |
| **Cronograma** | Linha do tempo de entregas: etapa, título, tags e resultado esperado. |
| **Precificação** | O investimento, montado em sub-blocos. Ver **[Precificação por Blocos](/modulos/precificacao/)**. |
| **Razões para a parceria** | Lista de diferenciais e provas — por que fechar com você. Também aceita a escolha de **cards por linha**. |
| **Grid de cards** | Cards com ícone ou imagem — benefícios, números, destaques — com **cards por linha** configurável (2, 3 ou 4). |
| **Callout / Citação** | Caixa de destaque ou citação com atribuição (prova social). Aceita uma **foto/avatar opcional** de quem depõe — ideal para depoimentos. |
| **Comparação de investimento** | Valor de mercado riscado × o seu valor × economia — ancoragem de preço. |

### Escrever com formatação

Os campos de texto corrido do editor têm a **barra de formatação do WordPress** — a mesma que você já conhece de páginas e posts. Você aplica **negrito**, *itálico*, sublinhado, listas com marcadores ou numeradas, links e alinhamento, e **o resultado aparece na hora, no próprio campo**: o que você vê enquanto escreve é o que o cliente vai ver na proposta.

![Bloco de Texto com o editor de texto formatado e sua barra de ferramentas](/assets/screenshots/editor-bloco-texto-rico.png)

O editor formatado está em:

- o bloco de **Texto**;
- a **descrição** de cada item das **Razões para a parceria**;
- o texto de cada card do **Grid de cards**;
- o texto do **Callout / Citação**;
- a **descrição** de cada item de **Produtos e Serviços**.

Na barra você também escolhe entre **Parágrafo**, **Subtítulo** e **Subtítulo menor**. Não existem níveis maiores de título de propósito: eles competiriam com os títulos de seção da própria proposta e bagunçariam a hierarquia visual.

{: .note }
> **Não é mais preciso escrever com asteriscos**
>
> Até a versão 1.23, a formatação era escrita com marcadores no meio do texto (`**negrito**`) e só aparecia depois, na proposta publicada. Agora você formata clicando nos botões. **Todo o conteúdo escrito daquele jeito foi convertido automaticamente** e continua aparecendo exatamente como antes — não há nada para refazer.

## Descrição e entregáveis, em Produtos e Serviços

Cada item do bloco **Produtos e Serviços** tem dois campos de conteúdo, com papéis diferentes:

| Campo | O que é |
|---|---|
| **Descrição (parágrafo introdutório)** | Um parágrafo que **apresenta** o produto — o que ele é, para quem serve, que problema resolve. Aceita formatação. |
| **Entregáveis / Lista de Recursos** | A **lista** do que está incluído. Um entregável por linha; cada linha vira um item da lista no card. |

![Campos de descrição e entregáveis num item de Produtos e Serviços](/assets/screenshots/editor-produto-descricao.png)

A distinção é simples: a descrição **conta**, os entregáveis **listam**. Um card fica bom com os dois — o parágrafo dá o contexto, a lista dá a concretude.

{: .warning }
> **Ao importar do catálogo, a descrição do catálogo vira a lista de entregáveis**
>
> Isso costuma confundir. Quando você usa **Importar do Catálogo**, a descrição cadastrada no item do catálogo é quebrada **linha a linha** e entra como **entregáveis** — porque é assim que o catálogo é preenchido na prática, uma linha por item entregue.
>
> O **parágrafo introdutório é escrito à mão**, na proposta, e vem vazio na importação. Se o card importado ficou só com uma lista e você quer uma apresentação antes dela, preencha o campo **Descrição** depois de importar.

## Quantos cards por linha

Nos blocos de **Produtos e Serviços**, **Razões para a parceria** e **Grid de cards**, você define quantos cards ficam lado a lado: **2, 3 ou 4**.

O número escolhido é um **limite, não uma obrigação**. Se houver menos cards do que colunas, eles crescem e ocupam a largura toda em vez de deixar um vazio à direita. Se houver mais, eles quebram para a linha seguinte — e, quando sobra um card sozinho na última linha, ele também se estica para preencher.

No celular, os cards sempre aparecem um por linha, independentemente da configuração.

{: .tip }
> **A ordem conta uma história**
>
> Uma sequência que funciona: **Capa → Texto (a dor) → Produtos (a solução) → Cronograma (o caminho) → Comparação/Precificação (o investimento) → Razões (a confiança)**. Guie o cliente do problema ao "sim".

### Reaproveitar conteúdo da Biblioteca

Textos que se repetem entre propostas — apresentação da empresa, razões da parceria, depoimentos — não precisam ser reescritos. No construtor, o botão **"+ Da Biblioteca"** insere um conteúdo salvo como um bloco editável (uma cópia; alterar aqui não muda o original). E, em cada bloco de Texto, Razões, Grid ou Callout, a ação **"Salvar na biblioteca"** faz o caminho inverso — guarda aquele bloco como um conteúdo reutilizável. A biblioteca fica no **[Catálogo → aba Conteúdos](/modulos/conteudos/)**.

### A capa vem do bloco Hero

Não existe um campo solto de "capa": o **primeiro bloco Hero** da lista é o que define a capa da página e o título que aparece na aba do navegador. Sem Hero, a proposta usa um título padrão. Para uma capa com imagem de fundo, ative **"Usar a imagem como fundo da capa"** no Hero.

## Aba Comentários

Mostra a conversa de negociação com o cliente. As perguntas feitas na proposta pública chegam aqui, e você responde no mesmo lugar. Detalhes em **[Acompanhar, Responder e Fechar](/guia/acompanhar/)**.

![Aba de comentários com a negociação](/assets/screenshots/editor-comentarios.png)

## Aba Histórico

Reúne a auditoria da proposta: o **Certificado de Aceite Digital** (quando aceita), o **histórico de versões** e o **log de visualizações** do cliente. Ver **[A Proposta Pública e o Aceite](/modulos/proposta-publica/)**.

## Salvar e publicar

No rodapé: **Salvar rascunho**, **Salvar e publicar** e, em propostas já existentes, **Publicar como Nova Versão**. Há ainda o botão **Visualizar Proposta**, que abre a página pública em nova aba.
