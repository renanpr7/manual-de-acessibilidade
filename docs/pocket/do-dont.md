# Do e Don't

Cada par mostra o jeito certo (Do) e o errado (Don't) de implementar itens do checklist, na mesma ordem das seções.

## Imagens

```html
<!-- DO -->
<img src="grafico.png" alt="Gráfico de barras: matrículas cresceram de 120 em 2024 para 180 em 2025">
<img src="borda.png" alt="">
<a href="https://instagram.com/unb"><img src="ig.svg" alt="Instagram da UnB"></a>

<!-- DON'T -->
<img src="grafico.png">
<img src="borda.png" alt="imagem decorativa bonita">
<a href="https://instagram.com/unb"><img src="ig.svg" alt="ícone"></a>
```

## Links e botões

```html
<!-- DO -->
<a href="/relatorio-2025.pdf">Baixe o relatório anual 2025 (PDF, 2 MB)</a>
<button type="button" aria-label="Fechar aviso">×</button>
<button type="button" onclick="ativarContraste()">Alto contraste</button>

<!-- DON'T -->
<a href="/relatorio-2025.pdf">Clique aqui</a>
<span class="x" onclick="fechar()">×</span>
<a href="#" onclick="ativarContraste()">Alto contraste</a>
```

## Foco e teclado

```html
<!-- DO -->
<a class="pular" href="#conteudo">Pular para o conteúdo</a>
<main id="conteudo">…</main>
<style>
  :focus-visible { outline: 3px solid #1a4fd6; outline-offset: 2px; }
</style>

<!-- DON'T -->
<style>
  *:focus { outline: none; }
</style>
```

## Títulos e regiões

```html
<!-- DO -->
<header>…</header>
<nav aria-label="Menu principal">…</nav>
<main>
  <h1>Transparência</h1>
  <h2>Orçamento</h2>
  <h3>Despesas 2025</h3>
</main>
<footer>…</footer>

<!-- DON'T -->
<div class="topo">…</div>
<div class="titulo-grande">Transparência</div>
<h4>Orçamento</h4>
```

## Formulários

```html
<!-- DO -->
<label for="email">E-mail (obrigatório)</label>
<input id="email" type="email" autocomplete="email" required
       aria-describedby="email-erro" aria-invalid="true">
<p id="email-erro" role="alert">E-mail inválido. Use o formato nome@dominio.com.</p>

<fieldset>
  <legend>Período de admissão</legend>
  <label for="ini">Data inicial (DD/MM/AAAA)</label> <input id="ini" type="date">
  <label for="fim">Data final (DD/MM/AAAA)</label> <input id="fim" type="date">
</fieldset>

<!-- DON'T -->
<input type="text" placeholder="E-mail*">
<span style="color:red">Erro</span>
```

## Tabelas

```html
<!-- DO -->
<table>
  <caption>Senadores em exercício por estado</caption>
  <tr><th scope="col">Nome</th><th scope="col">Partido</th><th scope="col">UF</th></tr>
  <tr><td>Fulano de Tal</td><td>ABC</td><td>DF</td></tr>
</table>

<!-- DON'T -->
<table>
  <tr><td><b>Nome</b></td><td><b>Partido</b></td><td><b>UF</b></td></tr>
</table>
```

## Componentes customizados e status

```html
<!-- DO -->
<button aria-expanded="false" aria-controls="submenu">Serviços</button>
<ul id="submenu" hidden>…</ul>
<div role="status">12 resultados encontrados</div>

<!-- DON'T -->
<div class="menu" onmouseover="abrir()">Serviços</div>
<div class="resultado">12 resultados encontrados</div>
```

## Cor, contraste e zoom

```html
<!-- DO -->
<p><span aria-hidden="true">✔</span> Aprovado</p>
<p style="color:#595959; background:#ffffff">Texto com contraste 7:1</p>
<meta name="viewport" content="width=device-width, initial-scale=1">

<!-- DON'T -->
<p style="color:green">Aprovado</p>
<p style="color:#aaaaaa; background:#ffffff">Texto com contraste 2,3:1</p>
<meta name="viewport" content="width=device-width, maximum-scale=1, user-scalable=no">
```

## Animação

```css
/* DO */
@media (prefers-reduced-motion: reduce) {
  * { animation: none !important; transition: none !important; scroll-behavior: auto !important; }
}
/* + botão visível "Pausar carrossel" */

/* DON'T: carrossel que gira sozinho a cada 3 s sem pausa */
```

## Conteúdo

| Do | Don't |
| --- | --- |
| "Envie o formulário até 30/11." | "O formulário deverá ser enviado impreterivelmente até o último dia do mês corrente." |
| "Pessoa com deficiência visual" | "Portador de deficiência", "deficiente" |
| #AcessibilidadeDigital | #acessibilidadedigital |
| Alt: "Foto de estudantes em sala de aula da UnB, conversando em grupo" | Alt: "A foto mostra pessoas bonitas" |
