# Ferramentas e Técnicas

Ferramentas automáticas aceleram a avaliação, mas não substituem o teste manual, e as técnicas do W3C mostram como cumprir cada critério do checklist.

## Documentos técnicos do WCAG 2.2

- [WCAG 2.2 – tradução autorizada pt-BR](https://www.w3.org/Translations/WCAG22-pt-BR/): texto normativo com os 86 critérios de sucesso.
- [Understanding WCAG 2.2](https://www.w3.org/WAI/WCAG22/Understanding/): explica a intenção, os benefícios e exemplos de cada critério.
- [Techniques for WCAG 2.2](https://www.w3.org/WAI/WCAG22/Techniques/): técnicas suficientes e recomendadas e falhas comuns para cada critério.
- [How to Meet WCAG 2.2 (Quick Reference)](https://www.w3.org/WAI/WCAG22/quickref/): lista filtrável por nível e tecnologia, com links para critérios e técnicas.
- [ARIA Authoring Practices Guide (APG)](https://www.w3.org/WAI/ARIA/apg/): padrões de teclado e ARIA para componentes customizados (menus, abas, modais), referência normativa da NBR 17225.
- [ACT Rules](https://www.w3.org/WAI/standards-guidelines/act/rules/): regras de teste padronizadas usadas por ferramentas como axe.

**Prefixos das técnicas:** G = geral, H = HTML, C = CSS, ARIA = WAI-ARIA, SCR = script, F = falha (o que não fazer).

## Ferramentas de avaliação de acessibilidade

| Ferramenta | Tipo | O que verifica | Seções do checklist |
| --- | --- | --- | --- |
| [WAVE](https://wave.webaim.org/) | Extensão, auditoria automática | Alt ausente, contraste, títulos, rótulos, regiões, ARIA | Desenvolvimento, Design |
| [axe DevTools](https://www.deque.com/axe/devtools/) | Extensão, regras ACT | Critérios WCAG A/AA no código, nomes acessíveis | Desenvolvimento |
| [Google Lighthouse](https://developer.chrome.com/docs/lighthouse/) | DevTools do Chrome | Pontuação geral de acessibilidade | Visão geral |
| [Accessibility Insights for Web](https://accessibilityinsights.io/docs/web/overview/) | Extensão, auditoria guiada | Teste rápido e roteiro de ordem de foco | Teclado e foco |
| [ASES Web](https://asesweb.governoeletronico.gov.br/) | Avaliador do governo (eMAG) | Código e acessibilidade de sites públicos brasileiros | Visão geral |
| [Access Monitor Plus](https://accessmonitor.acessibilidade.gov.pt/) | Avaliador online | Erros por critério WCAG | Visão geral |
| [W3C Markup Validation](https://validator.w3.org/) | Validador de HTML | Erros de marcação | Semântica e estrutura |
| [HeadingsMap](https://chromewebstore.google.com/search/HeadingsMap) | Extensão | Estrutura de títulos e regiões | Semântica e estrutura |
| [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/) | Contraste | Razão de contraste texto/fundo | Cor e contraste |
| [Colour Contrast Analyser](https://www.tpgi.com/color-contrast-checker/) | Programa | Contraste com conta-gotas, inclusive sobre imagens | Cor e contraste |
| [Colorblindly](https://github.com/oftheheadland/Colorblindly) | Simulador de daltonismo | Informação só por cor | Cor e contraste |
| [NVDA](https://www.nvaccess.org/) | Leitor de tela (Windows, gratuito) | Nomes, estados, ordem e mensagens anunciadas | Todas |
| [VoiceOver](https://support.apple.com/pt-br/guide/voiceover/welcome/mac) / [TalkBack](https://support.google.com/accessibility/android/answer/6283677?hl=pt-BR) | Leitor de tela móvel | Navegação por toque | Desenvolvimento, Design |
| [Funkify](https://www.funkify.org/) | Simulador de deficiências | Tremor, visão embaçada, dislexia | Design empático |

## Ferramentas de UX

| Ferramenta | Uso no guia |
| --- | --- |
| [Miro](https://miro.com/) ou [FigJam](https://www.figma.com/figjam/) | Mapas de empatia, jornadas, blueprints e canvas em quadro colaborativo |
| [Figma](https://www.figma.com/) + plugin [Stark](https://www.getstark.co/) | Protótipos com verificação de contraste, ordem de foco e simulação de daltonismo |
| [UXPressia](https://uxpressia.com/) | Modelos prontos de personas, jornadas e blueprints |
| [Lean UX Canvas](https://jeffgothelf.com/blog/leanuxcanvas-v2/) | Modelo do canvas citado na seção de [UX](ux.md#canvas) |

## Roteiro mínimo de verificação manual

1. Navegue a página só com Tab, Shift+Tab, Enter, Espaço e Esc.
2. Inspecione elementos interativos no DevTools para confirmar a semântica.
3. Percorra a página com o NVDA (títulos com H, regiões com D, links com K).
4. Meça contraste e teste zoom de 200% e largura de 320 px.
5. Repita os passos principais no celular com TalkBack ou VoiceOver.
