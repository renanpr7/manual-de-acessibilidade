# UX e Design Centrado no Usuário

Acessibilidade é parte da experiência do usuário: os artefatos abaixo garantem que pessoas com deficiência entrem no projeto desde a pesquisa, e não só na correção final. A base é o design centrado no ser humano da ABNT NBR ISO 9241-210, a usabilidade da ABNT NBR ISO 9241-11 (eficácia, eficiência e satisfação) e a abordagem prática de Design de Serviço de **Stickdorn et al. (2019)**.

## Design empático (mapa de empatia)

O mapa de empatia organiza o que o usuário **diz, pensa, faz e sente**, além de suas dores e ganhos, a partir de pesquisa com pessoas reais.

- **Basear o mapa em pesquisa real** (entrevista, observação, depoimento), não em suposições da equipe.
- **Incluir pelo menos um mapa de pessoa com deficiência** e registrar a tecnologia assistiva que ela usa.
- **Registrar barreiras e frustrações concretas** (ex.: "o leitor de tela não anuncia o botão de enviar").
- **Usar exercícios de simulação** (navegar sem mouse, com leitor de tela, sem som) para a equipe sentir as barreiras, sem substituir a escuta de pessoas com deficiência.

## Personas

Personas são perfis fictícios construídos a partir da pesquisa, com objetivos, contexto, habilidades e frustrações.

- **Criar personas a partir de dados de pesquisa**, não de estereótipos.
- **Incluir personas com deficiência visual, auditiva, física e cognitiva**, além de pessoa idosa e de baixo letramento digital.
- **Descrever em cada persona** o dispositivo, a tecnologia assistiva, o nível de letramento digital e o contexto de uso (ex.: celular de baixo desempenho, internet móvel).
- **Escrever objetivos e tarefas da persona no site**, que depois guiam jornadas e testes.
- **Tratar a deficiência como contexto**, não como a identidade inteira da persona.

## Jornada do usuário

O mapa de jornada mostra, etapa por etapa, o que a persona faz para cumprir um objetivo, por quais canais, o que sente e onde encontra barreiras.

- **Mapear a jornada de cada persona** para as tarefas principais do site (ex.: encontrar uma informação, preencher um formulário).
- **Registrar em cada etapa:** ações, pontos de contato, pensamentos, emoções e barreiras de acessibilidade.
- **Identificar os momentos críticos** (onde a pessoa desiste) e ligá-los a itens do checklist.
- **Considerar canais além do site** (atendimento telefônico, presencial, e-mail) quando fazem parte da jornada.
- **Destacar os "Momentos da Verdade" (moments of truth)** segundo Stickdorn et al. (2019) nas tarefas principais do portal (ex.: consultar um Projeto de Lei, assistir a uma sessão em vídeo ou enviar mensagem pelo Fale Conosco).

## Service Blueprint

O blueprint de serviço detalha a jornada em cinco camadas principais: evidências físicas e digitais, ações do usuário, pontos de contato visíveis (frontstage), ações internas (backstage) e processos de apoio, separados pelas linhas de interação, de visibilidade e de interação interna (Stickdorn et al., 2019).

- **Partir de uma jornada já mapeada** e acrescentar as camadas de evidências físicas/digitais, frontstage, backstage e processos de apoio (Stickdorn et al., 2019).
- **Indicar onde a acessibilidade depende de processos internos (backstage e suporte)** (ex.: fluxo editorial de publicação de texto alternativo, legendagem de vídeos, geração de PDFs com OCR/tags e integração com sistemas legados ou APIs).
- **Marcar pontos de falha e de espera** que afetam mais as pessoas com deficiência (ex.: limite de tempo, validação presencial obrigatória, CAPTCHA sem alternativa acessível ou documento sem texto selecionável).

## Canvas

Canvas são quadros de uma página que alinham a equipe. Os mais usados em UX são o **Lean UX Canvas** (problema, usuários, resultados, hipóteses) e o **Canvas de Proposta de Valor** (tarefas, dores e ganhos do usuário x produto).

- **Escrever o problema de negócio e o problema do usuário** incluindo as barreiras de acesso.
- **Listar entre os usuários as personas com deficiência.**
- **Definir resultados mensuráveis**, incluindo a meta de conformidade (ex.: WCAG 2.2 AA).
- **Escrever hipóteses e como validá-las com usuários reais.**

## Do artefato ao checklist

| Artefato | Pergunta que responde | Onde aparece no guia |
| --- | --- | --- |
| Mapa de empatia | Como a pessoa vive a barreira? | [Conscientização](conscientizacao.md) |
| Personas | Para quem estamos projetando? | Conscientização e Concepção |
| Jornada | Em que etapa a pessoa trava? | Desenvolvimento, Design, Conteúdo |
| Blueprint | Que processo interno causa a barreira? | Desenvolvimento e Conteúdo |
| Canvas | Que resultado o projeto persegue? | Planejamento de UX e Metas WCAG |

Material de apoio: esta seção explica esses procedimentos e não entra na contagem do checklist.
