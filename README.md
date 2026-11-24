# Claude como gestor de agentes â€” curso ARCKHÉ v7.2

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


Saia do chat: coordene uma equipe de agentes no Claude. Oito aulas curtas, abertas e gratuitas:
sessÃµes em segundo plano e agent view, a sessÃ£o gestora, Projects na nuvem, artifacts, custo e controle
(`/skill-doctor`, `/usage`, `/advisor`, status line, mods) e o seu sistema de gestÃ£o.

**Curso:** https://linnoff88-dev.github.io/

| # | Aula | PÃ¡gina |
|---|---|---|
| 1 | A virada: do chat Ã  gestÃ£o | `aulas/virada/` |
| 2 | A sessÃ£o por dentro (`/btw`, `/recap`, `/color`, tela dividida) | `aulas/sessao/` |
| 3 | SessÃµes em segundo plano (`claude --bg`, `claude agents`) | `aulas/segundo-plano/` |
| 4 | A sessÃ£o gestora: ela coordena, vocÃª decide | `aulas/sessao-gestora/` |
| 5 | Local, segundo plano ou nuvem (Projects) | `aulas/nuvem/` |
| 6 | Artifacts: do resultado ao link | `aulas/artifacts/` |
| 7 | Custo e controle | `aulas/custo/` |
| 8 | Seu sistema de gestÃ£o de agentes | `aulas/sistema/` |

Cada aula tem um explicavideo com o avatar do Nei (canal ARCKHÉ, lives7).

## O processo, do inÃ­cio ao fim

Legenda: ðŸ§  sessÃ£o com o Nei Â· âš™ï¸ script/timer Â· ðŸ¤– `claude -p` / subagente

1. ðŸ§  Pedido do Nei + conteÃºdo de origem â†’ fatos conferidos na documentaÃ§Ã£o oficial (`longrun/2026-10-28-claude-gestor-agentes/FATOS.md` no repo wifi).
2. âš™ï¸ Criar o curso: `~/.claude/skills/formato-curso-v72/scripts/novo-curso.sh ~/projetos/claude-gestor-de-agentes-v72 "Claude como gestor de agentes"`.
3. ðŸ¤– Escrever as aulas em `conteudo/pt/aulas/*.json` (um redator por par de aulas, sÃ³ com fatos do FATOS.md).
4. ðŸ¤– Imagens: capa e fotos de abertura pelo Codex (`codex exec`, image_gen na assinatura) â†’ `assets/img/`.
5. âš™ï¸ PortÃ£o: `python3 gerar.py && python3 validar.py --links && node ~/.claude/skills/formato-curso-v72/scripts/conferir-tela.cjs .`
6. ðŸ¤– Revisor independente (agente novo, persona do pÃºblico) â†’ corrigir â†’ revisar de novo; notas em `~/projetos/wifi/scripts/revisor-nota.py`.
7. âš™ï¸ Publicar: commit + `gh repo create linnoff88-dev/claude-gestor-de-agentes-v72 --public --source . --push` + GitHub Pages da raiz.
8. ðŸ¤– Explicavideos: roteiro, visual e capa por aula (`~/projetos/output/claude-gestor-agentes-videos/cga-aN/`).
9. âš™ï¸ Avatar no estÃºdio HeyGen + render: `tools/lote.sh cga-aN â€¦` (longrun) â†’ `entrega/cga-aN.mp4`.
10. âš™ï¸ YouTube lives7 + bot v3 + ARCKHÉytbot: `tools/plano16.sh` (dry-run) â†’ `tools/publica16.sh` (ou `tools/auto.sh`).
11. âš™ï¸ VÃ­deos no curso: release `video-v1.0.0` + `tools/embute.py` â†’ `gerar.py` â†’ push.
12. âš™ï¸ Portal: skill `atualiza-portal` (curso em `courses.ts` + trilha Agentes Jarvis + enrichment) e vÃ­deos em `videoUpdatesData`.
13. ðŸ§  r7ex 9:16 da novidade: `~/projetos/r7ex/edicoes/2026-10-28-claude-gestor-agentes/` â†’ `producao/producao.py --add` â†’ fila do lives7.
14. ðŸ§  Telegram ARCKHÉ.CCODE (skill `postar-telegram`) + MENU.

## Mais no ARCKHÉ AI
- [Ficha completa deste curso](https://www.ARCKHÉ AI/cursos/388-claude-como-gestor-de-agentes-saia-do-chat-e-coordene-uma-equipe-de-agentes/)
- [Guia: como aprender inteligÃªncia artificial](https://www.ARCKHÉ AI/aprender-inteligencia-artificial/)
- [Todos os cursos](https://www.ARCKHÉ AI/cursos/)

ConteÃºdo aberto e gratuito Â· formato ARCKHÉ Learning v7.2 Â· ARCKHÉ AI

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>