---
title: Manual do Usuário
nav_order: 2
---

# 📖 Manual do Usuário — V3RProp

Bem-vindo ao **V3RProp**, o plugin WordPress definitivo para geração de propostas comerciais de alto impacto visual, com suporte a aceite eletrônico com validade jurídica, biblioteca de templates visuais, versionamento inteligente de propostas e integração REST API completa para plataformas de automação (como n8n).

Este manual descreve todas as funcionalidades do plugin e demonstra passo a passo como utilizá-las de forma otimizada.

---

## 📌 1. Visão Geral, Painel de Propostas e Dashboard Analítico

Ao acessar o menu **V3RProp** no menu lateral do seu WordPress, você será apresentado ao Painel de Propostas, que se divide em duas grandes áreas:

### 1.1. Dashboard Analítico de Métricas
No topo do painel, você terá acesso a um dashboard tático atualizado em tempo real. Você pode filtrar os dados por períodos específicos (ex: Últimos 30 dias, Mês Atual, Ano Atual, etc.).
* **Taxa de Conversão:** O percentual de propostas que foram aceitas eletronicamente.
* **Receita (Ganhos):** O valor financeiro total de todas as propostas aprovadas.
* **Ticket Médio:** O valor médio das propostas aprovadas no período.
* **Pipeline (Abertas):** O valor em negociação que ainda aguarda aprovação ou recusa.
* **Gráficos Adicionais:** Acompanhe o **Funil de Propostas** para ver o volume de perda/ganho, um ranking dos **Top Clientes** por receita gerada, e a lista de **Módulos Mais Vendidos**.

### 1.2. Listagem Dinâmica de Propostas
Abaixo dos indicadores, você acompanha o grid de todas as propostas.
* **Ações Rápidas:** Visualize, copie o link público, edite, duplique ou exclua propostas diretamente da lista.
* **Status da Proposta:** Acompanhe em tempo real se uma proposta está em *Rascunho (Draft)*, *Ativa (Active)*, *Aceita (Accepted)*, *Com Restrição (Rejected)* ou *Expirada (Expired)*.

![Painel Geral - Dashboard](/screenshots/screen_1_dashboard.png)

---

## 👥 2. Cadastro e Gestão de Clientes

Antes de criar uma proposta, é recomendável cadastrar o cliente destinatário para que os dados sejam preenchidos de forma consistente.

* No painel, clique na aba **Clientes**.
* Preencha as seguintes informações, auxiliadas por tooltips com exemplos:
  * **Razão Social e CNPJ:** Dados legais da organização parceira. O campo de CNPJ suporta automaticamente o novo formato Alfanumérico instituído pela Receita Federal (ex: 12.ABC.345/01DE-35), aplicando a máscara corretamente em tempo real.
  * **Nome do Contato e E-mail Comercial:** O e-mail cadastrado aqui será usado para receber e-mails de notificação, visualização e comentários, e servirá como chave de segurança para acesso a áreas autenticadas de propostas.
  * **Telefone e Endereço:** Dados de contato e de cabeçalho do contrato.
  * **Logomarca do Cliente:** URL de uma imagem PNG com fundo transparente para ser exibida de forma destacada na capa da proposta.

### Tela de Cadastro de Cliente (Modal)
![Cadastro de Cliente](/screenshots/screen_2_client_modal.png)

### Lista de Clientes Cadastrados
![Lista de Clientes](/screenshots/screen_3_clients_list.png)

---

## ⚙️ 3. Configurações da Organização

A aba **Configurações** define os dados globais da sua própria empresa/organização comercial que emite as propostas.

* **Identidade da Organização:** Selecione a sua logomarca padrão utilizando a biblioteca de mídia nativa do WordPress (com upload de novos arquivos ou seleção de arquivos existentes) e acompanhe a pré-visualização instantânea (thumbnail).
* **E-mail Comercial de Recebimento:** Defina o endereço de e-mail de atendimento da sua organização. Todos os e-mails transacionais (como notificação de primeira visualização de proposta pelo cliente, novos comentários na proposta ou notificação de aceite eletrônico) serão enviados para este endereço ao invés do e-mail administrativo geral do WordPress.
* **Integração REST API (n8n):**
  * Gere chaves seguras aleatórias para integrar suas propostas com ferramentas externas como o n8n ou Make.
  * Copie a chave de API gerada para uso imediato em cabeçalhos HTTP.

![Configurações da Organização](/screenshots/screen_4_settings.png)

---

## ✏️ 4. O Editor de Propostas (Passo a Passo)

Ao criar ou editar uma proposta, você utilizará um editor estruturado por abas, focado em preenchimento dinâmico e livre de distrações. Todos os campos possuem **tooltips informativos** com orientações e exemplos em tempo real.

### Aba 1: Identidade & Layout
* **Cliente:** Selecione um dos clientes cadastrados para vincular à proposta.
* **Validade e Prazo:** Insira o prazo de validade da proposta comercial (em dias) e o prazo estimado de entrega do projeto (em meses).
* **Biblioteca de Templates Visuais:** Escolha um dos 5 presets de cores e fontes desenhados especificamente para propostas elegantes (ex: *RIT Clássico*, *Ocean Tech*, *Nordic Forest*, *Classic Luxury* e *Warm Sunset*). As cores primárias, secundárias e a Google Font do documento público standalone se adaptarão de forma instantânea.
* **Acesso Privado (Senha):** Adicione opcionalmente uma senha. Se preenchida, o cliente precisará digitá-la para visualizar a proposta no link público standalone.

![Aba Identidade & Layout](/screenshots/screen_5_editor_settings.png)

### Aba 2: Capa & Conteúdo
* Preencha o **Subtítulo (Kicker)** e o **Título Principal** da capa da proposta.
* Escreva o texto descritivo de apresentação institucional e objetivos, definindo com clareza o problema e a solução proposta.

![Aba Capa & Conteúdo](/screenshots/screen_6_editor_content.png)

### Aba 3: Módulos de Escopo
* Adicione cartões para detalhar o escopo da solução proposta.
* Cada card contém: Título, Número do Módulo e uma lista de atividades ou subitens específicos.
* **Reordenação de Módulos:** Permite alterar a sequência dos módulos facilmente através dos botões de setas (Mover para Cima / Mover para Baixo), sem a necessidade de excluir e recriar os itens.
* Na visualização pública, o escopo é automaticamente formatado em um grid harmonioso seguindo a ordem definida.

![Aba Módulos](/screenshots/screen_7_editor_modules.png)

### Aba 4: Cronograma de Entregas
* Defina as etapas mensais da execução física do projeto.
* Para cada mês, preencha o Título da Entrega, Tags (atividades principais do período) e o Resultado Esperado.
* **Reordenação de Marcos:** Permite reordenar a sequência das etapas facilmente usando os botões de setas (Mover para Cima / Mover para Baixo).
* O sistema renderiza uma linha do tempo vertical no documento público baseada na nova ordem.

![Aba Cronograma](/screenshots/screen_8_editor_timeline.png)

### Aba 5: Precificação e Condições (Orçamento)
* **Tabela de Investimento:** Adicione os itens de investimento detalhando descrição, valor de mercado e valor proposto (oferecido com desconto social). O sistema calcula de forma transparente a soma e o benefício (desconto total gerado para o terceiro setor).
* **Reordenação de Itens:** Permite mover itens para cima ou para baixo diretamente na tabela de precificação para estruturar a ordem de apresentação ao cliente.
* **Parcelamento Automático (Opcional):** Você pode habilitar o parcelamento automático da proposta. Ao fazer isso, basta informar a quantidade de parcelas desejada e se há algum acréscimo (percentual ou em valor fixo). O sistema recalcula automaticamente em tempo real o valor final parcelado e atualiza a descrição das condições de pagamento.
* **Condições de Pagamento e Impostos:** Defina a porcentagem de impostos incidentes e o texto personalizado de faturamento (caso o parcelamento automático esteja desabilitado).
* **Manutenção:** Especifique o valor da manutenção mensal ou semestral a ser iniciada após a conclusão do projeto.

![Aba Precificação](/screenshots/screen_9_editor_pricing.png)

---

## 🌐 5. Visualização Pública Standalone (Experiência do Cliente)

Ao salvar uma proposta, copie o link público. O seu cliente acessará uma página isolada de carregamento ultrarrápido com o design personalizado baseado no preset escolhido.

* **Navegação Sem Distrações:** Um layout focado 100% no conteúdo da proposta, livre de cabeçalhos ou menus normais do blog WordPress.
* **Sistema de Negociação por Comentários:** O cliente pode postar dúvidas ou observações no rodapé da página. Cada comentário gera uma notificação instantânea para o e-mail comercial da sua organização e envia uma confirmação de recebimento ao cliente. **Importante:** o envio de comentários/dúvidas não invalida a proposta (ela se mantém ativa e com status *Pendente*).
* **Solicitação de Alterações (Recusa):** Se o cliente rejeitar os termos ou precisar de mudanças estruturais, ele poderá abrir o formulário correspondente, preenchendo seu nome, e-mail e os motivos detalhados. A proposta muda para o status *Recusada*, notificando o comercial com os motivos informados e enviando uma confirmação ao cliente.
* **Aceite Eletrônico & PDF Assinado:** Um formulário seguro onde o decisor informa Nome Completo, E-mail Corporativo, CPF/CNPJ e assina o aceite comercial. Ao concluir:
  1. O sistema registra o timestamp exato, o endereço IP do assinante, o User-Agent (navegador/OS) e gera um código de autenticidade digital (hash MD5) de validade jurídica.
  2. Um PDF oficial completo da proposta é gerado automaticamente no servidor com um layout corporativo impecável e o certificado de assinatura eletrônica anexado ao final (com bordas finas de 0.5pt e quebras automáticas de linha para evitar cortes de texto).
  3. Ambos, o cliente e a equipe comercial (no e-mail definido nas Configurações da Organização), recebem uma cópia de e-mail de confirmação com este PDF assinado anexado.

![Proposta Standalone Pública](/screenshots/screen_10_proposal_public.png)

---

## 🔄 6. Versionamento Inteligente (Keep a Changelog)

Ao renegociar uma proposta comercial com o cliente, você pode editá-la e usar a opção **"Publicar como Nova Versão (Clonar)"**.

* A versão antiga é automaticamente arquivada como **Substituída (Superseded)**.
* Uma nova versão (ex: de v1 para v2) é criada e assume o endereço da URL pública.
* Caso o cliente acesse uma URL antiga substituída, o sistema exibe um aviso dinâmico informando que há uma versão comercial mais recente e atualizada, oferecendo um link direto para a versão vigente.

---

## 🔗 7. API REST Externa para Automações (n8n / Make)

O V3RProp conta com uma API REST externa robusta e segura para sincronização de cadastros e geração de propostas automáticas via fluxos de trabalho (ex: n8n, Make, HubSpot).

### Autenticação
Envie a sua chave de API nas requisições através do cabeçalho HTTP:
`X-V3RProp-API-Key: SUA_CHAVE_DE_API`

Ou por meio de parâmetro de URL:
`?api_key=SUA_CHAVE_DE_API`

### Endpoints Disponíveis
* `GET /wp-json/v3rprop/v1/external/clients` - Listar todos os clientes cadastrados.
* `POST /wp-json/v3rprop/v1/external/clients` - Cadastrar ou atualizar dados de um cliente.
* `GET /wp-json/v3rprop/v1/external/proposals` - Listar todas as propostas ativas no sistema.
* `POST /wp-json/v3rprop/v1/external/proposals` - Criar ou atualizar uma proposta comercial vinculada a um cliente.

---

## ⏰ 8. Automação de Lembretes e Expiração de Propostas

O V3RProp cuida automaticamente do follow-up com o cliente, garantindo que as propostas tenham prazos controlados e não fiquem "soltas" eternamente.

* **Cálculo em Dias Úteis:** O sistema considera o número de dias úteis para calcular a data final da proposta, pulando finais de semana.
* **Lembrete de 5 dias:** Faltando exatamente 5 dias úteis para a validade da proposta expirar, o cliente recebe um e-mail automatizado de acompanhamento.
* **Lembrete de Véspera:** Faltando apenas 1 dia útil, um último aviso de urgência é enviado, estimulando o aceite eletrônico.
* **Expiração Oficial:** Quando a data limite for alcançada e nenhum aceite ocorrer, a proposta muda o status para *Expirada*. Um e-mail de fechamento é enviado informando que a proposta não tem mais validade jurídica, orientando o cliente a contatar o comercial caso queira novas negociações.
* **Notificação (Cópia Oculta):** O e-mail administrativo configurado em *Configurações da Organização* sempre receberá uma cópia oculta (BCC) de todas as automações enviadas para manter a equipe ciente.

---

## 📊 9. Integração do Dashboard no Frontend (Shortcode)

Você pode exibir o Dashboard Analítico de Métricas diretamente em páginas públicas ou áreas logadas do seu site (frontend).
Basta utilizar o seguinte shortcode:

`[v3rprop_dashboard]`

O painel será renderizado com as mesmas métricas e gráficos que você vê no WP Admin.
*Dica de Segurança:* Este shortcode não possui controle de acesso nativo. Se você deseja que apenas gestores vejam o dashboard, restrinja o acesso da página onde o shortcode foi inserido através de plugins de membros ou controles de visibilidade da própria página.

---

## ✉️ 10. E-mails Transacionais Customizados

Nas Configurações Globais (aba **E-mails Transacionais**), você pode alterar o texto enviado ao cliente em cada estágio.
Utilize as seguintes chaves dinâmicas nos seus templates para personalizar as mensagens:
* `{NOME_DO_CLIENTE}`: Nome do decisor cadastrado.
* `{TITULO_DA_PROPOSTA}`: Título que você definiu na capa da proposta.
* `{LINK_DA_PROPOSTA}`: A URL do documento standalone.

Se você preferir os textos originais, basta limpar os campos que o V3RProp voltará a utilizar o padrão nativo otimizado. Além disso, existe o *Toggle* de ativação (enviar ou não e-mail na publicação) e um aviso se o cliente não tiver e-mail.

---

## 🔐 11. Assinatura Digital ICP-Brasil (Avançado)

A funcionalidade mais segura para fechar grandes contratos. O V3RProp permite assinar de forma autônoma os PDFs finais (quando a proposta é aceita eletronicamente pelo cliente) através de um Certificado Digital A1.

* Vá até as configurações em **Assinatura Digital (ICP-Brasil)**.
* Envie seu arquivo `.pfx` ou `.p12` e insira a respectiva senha.
* **Alertas de Expiração:** O V3RProp te avisará com 15, 5 e 1 dias de antecedência quando o seu certificado A1 estiver próximo do vencimento, permitindo tempo hábil para renovação. Quando o vencimento ocorrer, a assinatura digital é temporariamente suspensa voltando à assinatura eletrônica por IP/Hash (com validade legal).
