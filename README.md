

<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <h5>Projeto Basquete — Acessibilidade</h5>
  <link rel="stylesheet" href="style.css">
</head>
<body>
      <div>
        <h1>Projeto Basquete</h1>
        <div class="description">Tudo sobre o esporte e acessibilidade digital</div>
      </div>
    </div>
    <nav aria-label="Menu principal">
      <button class="btn" id="open-a11y" aria-haspopup="true" aria-controls="a11y-title">
        Menu de Acessibilidade
      </button>
    </nav>
  </header>

  <main id="main">
    <div class="grid">
      <section class="card">
        <div class="section">
          <h3>Como funciona o basquete</h3>
          <p>O basquete é um esporte coletivo jogado entre duas equipes de cinco jogadores. O objetivo é marcar pontos arremessando a bola dentro da cesta adversária. Cada partida é dividida em quatro períodos e envolve fundamentos como drible, passe, arremesso e defesa.</p>
        </div>
        <div class="section">
          <h3>Principais campeonatos</h3>
          <ul>
            <li><strong>NBA (EUA):</strong> maior liga profissional do mundo.</li>
            <li><strong>NBB (Brasil):</strong> Novo Basquete Brasil, principal campeonato nacional masculino.</li>
            <li><strong>EuroLeague:</strong> competição europeia de alto nível.</li>
            <li><strong>Jogos Olímpicos:</strong> torneio internacional realizado a cada quatro anos.</li>
          </ul>
        </div>
        <div class="section">
          <h3>Melhores jogadores</h3>
          <p>Ao longo da história, vários atletas se destacaram no basquete:</p>
          <ul>
            <li><strong>Michael Jordan</strong> — considerado o maior jogador de todos os tempos.</li>
            <li><strong>LeBron James</strong> — ícone da era atual.</li>
            <li><strong>Kobe Bryant</strong> — símbolo de dedicação e técnica refinada.</li>
            <li><strong>Oscar Schmidt</strong> — brasileiro reconhecido mundialmente.</li>
            <li><strong>Larry Bird, Magic Johnson, Stephen Curry</strong> e outros.</li>
          </ul>
        </div>
      </section>
      <aside class="card" aria-labelledby="a11y-title">
        <h2 id="a11y-title">Menu de Acessibilidade</h2>
        <div class="a11y">
          <p class="note">Personalize a interface: tamanho da fonte, contraste e preferências.</p>
          <div>
            <label for="font-size-range">Tamanho da fonte</label>
            <div class="controls">
              <button class="btn" id="decrease-font" aria-label="Diminuir fonte">A-</button>
              <input id="font-size-range" type="range" min="12" max="22" step="1" value="16" aria-valuemin="12" aria-valuemax="22" aria-valuenow="16">
              <button class="btn" id="increase-font" aria-label="Aumentar fonte">A+</button>
            </div>
          </div>
          <div>
            <label for="contrast-toggle">Modo alto contraste</label>
            <div class="controls">
              <button class="btn" id="toggle-contrast" aria-pressed="false">Ativar contraste</button>
            </div>
          </div>
          <div>
            <label for="motion-toggle">Reduzir movimentos</label>
            <div class="controls">
              <button class="btn" id="toggle-motion" aria-pressed="false">Reduzir animações</button>
            </div>
          </div>
          <div>
            <button class="btn" id="reset" aria-label="Restaurar padrões">Restaurar padrões</button>
          </div>
          <div class="tip">Dica: as preferências são salvas no seu navegador.</div>
        </div>
      </aside>
    </div>
  </main>

  <div class="aria-status" aria-live="polite" id="a11y-status"></div>

  <footer>
    <small>© Projeto Basquete — Lucas Batista</small>
  </footer>

  <script src="script.js"></script>
</body>
</html>
