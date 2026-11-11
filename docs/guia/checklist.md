# Checklist

O checklist tem 143 itens. Veja em [Guia de Acessibilidade](index.md) como usá-lo e como ler os indicadores de nível. A aplicação deste checklist ao Portal da Câmara dos Deputados está em [Avaliação do Portal](../avaliacao-site/index.md).

## Desenvolvimento

### Teclado e foco

- [ ] **Exibir indicador de foco visível** em todos os elementos focáveis. (AA)
- [ ] **Evitar que o elemento em foco fique totalmente escondido** por cabeçalho fixo, banner de cookies ou chat. (AA)
- [ ] **Manter o elemento em foco completamente visível.** (AAA, Recomendação)
- [ ] **Garantir ordem de foco lógica** (Tab segue a ordem visual). (A)
- [ ] **Evitar armadilha de foco:** é possível entrar e sair de todo componente só com teclado. (A)
- [ ] **Permitir operar toda funcionalidade só pelo teclado**, exceto as que dependem do traçado (desenho à mão livre). (A)
- [ ] **Tornar toda funcionalidade acessível por teclado, sem exceção.** (AAA, Recomendação)
- [ ] **Abrir e fechar submenus pelo teclado**, não só por mouseover. (A)
- [ ] **Permitir desativar ou remapear atalhos de tecla única**, ou fazer com que só funcionem com o componente em foco. (A)
- [ ] **Manter visível e dispensável (Esc) o conteúdo exibido por hover ou foco** (tooltip, submenu). (AA)
- [ ] **Adicionar link "Pular para o conteúdo"** como primeiro item focável, ou outro mecanismo para contornar blocos repetidos. (A)
- [ ] **Dar instruções de uso para componentes customizados** de interação complexa. (A)

### Semântica e estrutura do código

- [ ] **Dar a cada página um `<title>` único e descritivo.** (A)
- [ ] **Declarar o idioma da página** (`lang="pt-BR"`). (A)
- [ ] **Marcar com `lang` trechos em outro idioma.** (AA)
- [ ] **Usar h1 a h6 nos títulos**, não apenas fonte grande ou negrito. (A)
- [ ] **Manter hierarquia de títulos lógica**, sem pular níveis (h2 para h4). (A)
- [ ] **Ter um, e só um, h1** que identifica a página. (AAA, Recomendação)
- [ ] **Usar regiões** (`header`, `nav`, `main`, `footer`) de acordo com o conteúdo. (A)
- [ ] **Dar nome acessível único a regiões do mesmo tipo** (ex.: dois `nav` com `aria-label` diferentes). (A)
- [ ] **Colocar todo o conteúdo em regiões**, com no máximo um header, um main e um footer. (AAA, Recomendação)
- [ ] **Usar `ul`, `ol` ou `dl` para listas** de itens da mesma natureza. (A)
- [ ] **Marcar tabelas de dados com `table`, `th` e `scope`** e não usar tabela para leiaute. (A)
- [ ] **Associar um título (`caption`) a cada tabela.** (A)
- [ ] **Manter a ordem do código (DOM) igual à ordem visual.** (A)
- [ ] **Preferir elementos nativos** (`button`, `a`, `input`) a `div` com clique. (A, Recomendação)
- [ ] **Expor função, estado e valor de componentes customizados** (`role`, `aria-expanded`, `aria-checked`). (A)
- [ ] **Dar nome acessível a todo componente que precisa de nome**, contendo o texto visível. (A)
- [ ] **Anunciar mensagens de status sem mover o foco** (`role="status"` ou `aria-live`). (AA)
- [ ] **Dar `title` único a todo `iframe`.** (A)
- [ ] **Não bloquear o zoom** (sem `user-scalable=no` ou `maximum-scale=1`). (AA)
- [ ] **Marcar ênfase, citação e abreviação** com `strong`, `em`, `blockquote`, `abbr`. (A)
- [ ] **Não inserir conteúdo relevante só por CSS** (`::before`) nem escondê-lo do leitor de tela com `display:none`. (Boa prática)

### Imagens (implementação)

- [ ] **Adicionar `alt` que descreve a informação** em imagens de conteúdo. (A)
- [ ] **Adicionar `alt` que descreve a ação ou o destino** em imagens funcionais (ícone em link ou botão). (A)
- [ ] **Usar `alt=""` ou CSS em imagens decorativas.** (A)
- [ ] **Dar descrição detalhada a imagens complexas** (gráficos, infográficos), ao lado ou em página indicada. (A)
- [ ] **Evitar imagens de texto**, salvo as essenciais (logotipo). (AA)
- [ ] **Adicionar texto alternativo em cada área de mapas de imagem.** (A)

### Links e navegação

- [ ] **Usar `<a href>` para navegar e `<button>` para ações.** (A)
- [ ] **Deixar claro o propósito do link** pelo texto ou pelo contexto (sem "clique aqui" isolado). (A)
- [ ] **Deixar claro o propósito do link só pelo texto do link.** (AAA, Recomendação)
- [ ] **Levar ao mesmo destino links com o mesmo texto.** (AA, Recomendação)
- [ ] **Avisar quando o link abre nova aba, baixa arquivo (formato e tamanho) ou leva a site externo.** (AAA, Recomendação)
- [ ] **Oferecer mais de uma forma de chegar a cada página** (menu, busca, mapa do site). (AA)
- [ ] **Manter a navegação repetida na mesma ordem** em todas as páginas. (AA)
- [ ] **Manter ajuda (contato, FAQ, chat) na mesma posição** em todas as páginas. (A)
- [ ] **Indicar onde o usuário está** (breadcrumb, item de menu ativo). (AAA, Recomendação)

### Botões e controles

- [ ] **Dar a todo botão texto ou nome acessível** que indica a função (inclusive botões só de ícone). (A)
- [ ] **Usar o mesmo nome para componentes com a mesma função** em todas as páginas. (AA)
- [ ] **Não mudar o contexto ao receber foco ou hover.** (A)
- [ ] **Não mudar o contexto ao alterar um campo ou `select`** sem aviso prévio. (A)
- [ ] **Disparar ações ao soltar o ponteiro**, com possibilidade de cancelar. (A)
- [ ] **Oferecer alternativa de toque simples a gestos** com vários dedos ou de traçado. (A)
- [ ] **Oferecer alternativa sem arrastar** a toda ação de arrastar (slider, reordenar, mapa). (AA)
- [ ] **Oferecer alternativa a funções por movimento do aparelho** e permitir desativá-las. (A)
- [ ] **Dar retorno perceptível quando um controle é acionado.** (AA, Recomendação)

### Formulários

- [ ] **Adicionar rótulo visível a todo campo** (placeholder não substitui rótulo). (A)
- [ ] **Associar o `label` ao campo** (`for` + `id`). (A)
- [ ] **Escrever rótulos e textos de ajuda descritivos**, em posição previsível. (AA)
- [ ] **Agrupar campos relacionados com `fieldset` e `legend`.** (A)
- [ ] **Indicar campos obrigatórios em texto** ou símbolo explicado, não só por cor. (A)
- [ ] **Adicionar autocomplete e tipo correto** em campos de dados pessoais. (AA)
- [ ] **Exibir mensagem de erro em texto** que diz qual é o erro e o campo, perto dele e anunciada pelo leitor de tela. (A)
- [ ] **Sugerir a correção na mensagem de erro** (ex.: "Use o formato DD/MM/AAAA"). (AA)
- [ ] **Permitir revisar, confirmar ou desfazer formulários críticos** (pagamento, dados jurídicos, exclusão). (AA)
- [ ] **Permitir revisar, confirmar ou desfazer todo formulário.** (AAA, Recomendação)
- [ ] **Não pedir de novo dados já informados** no mesmo processo, ou trazê-los preenchidos. (A)
- [ ] **Não exigir teste cognitivo no login:** permitir colar senha e usar gerenciador de senhas, ou oferecer alternativa. (AA)
- [ ] **Identificar o CAPTCHA e oferecer alternativa** em outra modalidade. (A)
- [ ] **Oferecer ajuda contextual** (instruções e exemplos) para preencher. (AAA, Recomendação)
- [ ] **Incluir botão de envio explícito em todo formulário.** (A, Recomendação)

### Tempo, movimento e modais

- [ ] **Permitir desligar, ajustar ou estender limites de tempo** antes de expirarem. (A)
- [ ] **Permitir pausar, parar ou ocultar animações automáticas** com mais de 5 s (carrossel, banner). (A)
- [ ] **Permitir pausar ou controlar atualizações automáticas** de conteúdo. (A)
- [ ] **Permitir pausar ou silenciar áudio** que toca sozinho por mais de 3 s. (A)
- [ ] **Evitar conteúdo que pisca mais de 3 vezes por segundo.** (A)
- [ ] **Evitar perda de dados quando a sessão expira**, ou avisar antes. (AAA, Recomendação)
- [ ] **Controlar o foco em modais:** entra no modal, fica nele enquanto aberto, fecha com Esc e com botão rotulado, volta ao gatilho. (Boa prática)
- [ ] **Não abrir modais sozinhos**, nem a partir de outro modal, nem em tela cheia. (Boa prática)

Itens cumpridos: \_\_\_\_ de 80.

## Design

Os itens de design verificam o que se vê na tela.

### Cor e contraste

- [ ] **Adicionar informação que não dependa exclusivamente da cor** (status, erro, legenda de gráfico). (A)
- [ ] **Distinguir links no meio do texto por algo além da cor** (ex.: sublinhado). (A)
- [ ] **Escrever instruções que não dependam só de forma, cor, tamanho, posição ou som** ("clique no botão verde à direita"). (A)
- [ ] **Garantir contraste de texto de pelo menos 4,5:1**; texto grande (18 pt ou 14 pt negrito) pelo menos 3:1. (AA)
- [ ] **Garantir contraste de texto aprimorado de 7:1**; texto grande 4,5:1. (AAA, Recomendação)
- [ ] **Garantir contraste de 3:1 em bordas de campos, botões e seus estados.** (AA)
- [ ] **Garantir contraste de 3:1 em ícones e partes de gráficos** necessárias para entender. (AA)
- [ ] **Garantir contraste de 3:1 no indicador de foco**, com o fundo e com o estado sem foco. (AA)
- [ ] **Usar indicador de foco com área de pelo menos o perímetro do elemento e 2 px de espessura.** (AAA, Recomendação)
- [ ] **Manter o contraste de texto sobre imagem ou degradê** nos pontos mais claro, médio e mais escuro. (AA)

### Tipografia e texto na tela

- [ ] **Tamanho do texto ajustável:** com zoom de 200% não há perda de conteúdo nem sobreposição. (AA)
- [ ] **Suportar espaçamento ajustado** (entrelinha 1,5×, parágrafo 2×, letras 0,12×, palavras 0,16×) sem cortar texto. (AA)
- [ ] **Parágrafos com no máximo 80 caracteres por linha**, ou largura ajustável. (AAA)
- [ ] **Evitar o alinhamento justificado**; alinhar à esquerda. (AAA, Recomendação)
- [ ] **Fontes são fluidas e de fácil entendimento**, sem textos longos em caixa alta, condensados ou manuscritos. (Boa prática)
- [ ] **Não reduzir a fonte padrão abaixo da do navegador** (16 px). (Boa prática)

### Leiaute e interação

- [ ] **Fazer com que as linhas se ajustem ao viewport:** com 320 px de largura não há rolagem horizontal nem perda de conteúdo. (AA)
- [ ] **Funcionar em retrato e em paisagem.** (AA)
- [ ] **Elementos interativos têm pelo menos 24×24 px ou espaçamento suficiente**, ou estão no texto, têm controle equivalente maior, ou o tamanho é essencial, legal ou definido pelo navegador. (AA)
- [ ] **Áreas clicáveis têm pelo menos 44×44 px.** (AAA, Recomendação)
- [ ] **Botões parecem botões e links parecem links**, de acordo com a função. (Boa prática)
- [ ] **Evitar excesso de informação e manter busca e menu sempre no mesmo lugar.** (Boa prática)
- [ ] **Preferir botões com texto e ícone**; botões apenas com ícone têm nome acessível. (Boa prática)
- [ ] **Oferecer opção de alto contraste (modo escuro) e aumento de fonte.** (Boa prática, não obrigatória)

### Animação

- [ ] **Permitir desativar animações disparadas pela interação** (parallax, zoom ao rolar), respeitando `prefers-reduced-motion`. (AAA, Recomendação)
- [ ] **Não ter conteúdo que pisque mais de 3 vezes em qualquer período de 1 s.** (AAA, Recomendação)
- [ ] **Usar animações só quando necessárias**, sem tela cheia e funcionando em velocidade reduzida. (Boa prática)

Itens cumpridos: \_\_\_\_ de 27.

## Geração de Conteúdo

Os itens de conteúdo verificam o que é publicado: textos, descrições de imagem, vídeos, áudios e arquivos.

### Texto e linguagem

- [ ] **Escrever títulos e rótulos que descrevem o tema ou o propósito.** (AA)
- [ ] **Usar linguagem simples**, frases curtas (15 a 20 palavras) e ordem direta. (AAA, Recomendação)
- [ ] **Explicar jargões, termos técnicos e expressões idiomáticas.** (AAA, Recomendação)
- [ ] **Escrever siglas por extenso na primeira vez** ou usar `abbr`. (AAA, Recomendação)
- [ ] **Indicar a pronúncia de palavras ambíguas** no contexto. (AAA, Recomendação)
- [ ] **Escrever links que dizem o destino ou a ação** ("Baixe o relatório 2025 (PDF, 2 MB)", não "baixar PDF"). (A)
- [ ] **Usar o termo "pessoa com deficiência"** (nunca "portador" ou "deficiente"). (Boa prática)
- [ ] **Usar pontuação correta** e evitar senso de urgência e figuras de linguagem desnecessárias. (Boa prática)
- [ ] **Escrever hashtags com maiúscula em cada palavra** (#AcessibilidadeDigital) e usar emojis com moderação. (Boa prática)

### Imagens (descrição)

- [ ] **Descrever no texto alternativo** o tipo de imagem, o quê ou quem aparece, onde e a ação, no presente. (A)
- [ ] **Evitar no alt** "a foto mostra", repetição do texto ao lado e juízo de valor. (Boa prática)
- [ ] **Dar alt curto e descrição longa fora do alt** para gráficos e infográficos. (A)
- [ ] **Publicar avisos, cartazes e banners como texto**, não como imagem de texto. (AA)

### Vídeo e áudio

- [ ] **Adicionar transcrição a áudio pré-gravado** (podcast) com falas, quem fala e sons relevantes. (A)
- [ ] **Adicionar legendas descritivas a vídeo pré-gravado** (falas, efeitos e sons de ambiente). (A)
- [ ] **Adicionar audiodescrição a vídeo pré-gravado**, ou garantir que o áudio original baste para entender sem ver. (AA)
- [ ] **Adicionar legendas a transmissões ao vivo.** (AA)
- [ ] **Adicionar transcrição completa (visual e sonora) a vídeos.** (AAA, Recomendação)
- [ ] **Adicionar janela de Libras**, à direita e com bom contraste. (AAA, Recomendação)
- [ ] **Oferecer audiodescrição estendida** quando o vídeo não tem pausas suficientes. (AAA, Recomendação)
- [ ] **Adicionar transcrição a áudio ao vivo.** (AAA, Recomendação)
- [ ] **Manter som de fundo baixo** (20 dB abaixo da fala) ou permitir desligá-lo. (AAA, Recomendação)
- [ ] **Acompanhar vídeos de um descritivo curto do conteúdo.** (Boa prática)

### Arquivos e conteúdo de terceiros

- [ ] **Publicar arquivos acessíveis** (PDF, DOCX com texto selecionável, títulos marcados, ordem de leitura correta). (Boa prática)
- [ ] **Escolher conteúdo de terceiros acessível** (vídeos e posts incorporados) ou avisar o usuário das barreiras. (Boa prática)
- [ ] **Oferecer informações importantes em mais de um formato** (texto + vídeo ou áudio). (Boa prática)

Itens cumpridos: \_\_\_\_ de 26.

## Heurísticas de Nielsen

As 10 heurísticas de Nielsen avaliam usabilidade e integram o checklist de avaliação do site. Marque a heurística quando o site a cumpre (critérios alinhados ao documento TG10 da equipe e diretrizes de e-Gov de Maciel e Medeiros, 2026):

- [ ] **1. Visibilidade do status do sistema:** o site mostra onde o usuário está (ex.: breadcrumbs, aba ativa) e dá retorno imediato e perceptível às ações (carregando, enviado, erro), tanto visualmente quanto para tecnologias assistivas (`role="status"` / `aria-live`).
- [ ] **2. Correspondência entre o sistema e o mundo real:** usa a linguagem do público cidadão, ícones reconhecíveis e ordem natural das informações, evitando jargões legislativos ou códigos técnicos de sistema sem explicação (ex.: "Erro 500").
- [ ] **3. Controle e liberdade do usuário:** há saídas claras para voltar, cancelar, desfazer ações e fechar modais, submenus e pop-ups (inclusive com a tecla Esc) sem perder o foco.
- [ ] **4. Consistência e padrões:** funções iguais têm o mesmo nome, cor, ícone e posição em todas as telas do portal, mantendo o menu principal e a busca padronizados e seguindo convenções da web.
- [ ] **5. Prevenção de erros:** o formato esperado é indicado antes do preenchimento, os dados são validados com máscaras/restrições, ações destrutivas pedem confirmação e a interface previne tanto deslizes (cliques acidentais) quanto enganos (instruções confusas), sem apagar os dados já preenchidos caso ocorra erro em um campo.
- [ ] **6. Reconhecimento em vez de memorização:** opções, regras de preenchimento e rótulos ficam permanentemente visíveis próximos aos campos (`<label>`, sugestões de busca) e o usuário não precisa lembrar informações entre telas.
- [ ] **7. Flexibilidade e eficiência de uso:** oferece caminhos claros e guiados para usuários iniciantes e disponibiliza aceleradores funcionais (atalhos de teclado accesskey, link "Pular para o conteúdo", busca rápida e preenchimento automático) para usuários experientes, funcionando com teclado, toque e tecnologias assistivas.
- [ ] **8. Estética e design minimalista:** não há informação irrelevante, excesso de banners ou pop-ups disputando atenção com os serviços principais, mantendo hierarquia visual clara e baixa carga cognitiva.
- [ ] **9. Ajudar o usuário a reconhecer, diagnosticar e recuperar-se de erros:** mensagens em linguagem simples indicam exatamente o campo com problema, dizem a causa sem códigos técnicos e sugerem como corrigir (ex.: "Use o formato DD/MM/AAAA"), sem perder o que foi preenchido.
- [ ] **10. Ajuda e documentação:** ajuda, FAQ, glossário legislativo, página de acessibilidade ou contato são fáceis de achar, ficam sempre no mesmo lugar e dão passos concretos e dicas contextuais.

Itens cumpridos: \_\_\_\_ de 10.

## Resumo do checklist

Ao final da avaliação, transfira para cá a contagem de cada seção.

| Seção | Itens cumpridos |
| --- | --- |
| Desenvolvimento | \_\_\_\_ de 80 |
| Design | \_\_\_\_ de 27 |
| Geração de Conteúdo | \_\_\_\_ de 26 |
| Heurísticas de Nielsen | \_\_\_\_ de 10 |
| **Total** | **\_\_\_\_ de 143** |
