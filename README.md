# Claude como gestor de agentes ê¢â¬â curso ARCKHê v7.2

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


Saia do chat: coordene uma equipe de agentes no Claude. Oito aulas curtas, abertas e gratuitas:
sessêÂµes em segundo plano e agent view, a sessêÂ£o gestora, Projects na nuvem, artifacts, custo e controle
(`/skill-doctor`, `/usage`, `/advisor`, status line, mods) e o seu sistema de gestêÂ£o.

**Curso:** https://linnoff88-dev.github.io/

| # | Aula | PêÂ¡gina |
|---|---|---|
| 1 | A virada: do chat êÂ  gestêÂ£o | `aulas/virada/` |
| 2 | A sessêÂ£o por dentro (`/btw`, `/recap`, `/color`, tela dividida) | `aulas/sessao/` |
| 3 | SessêÂµes em segundo plano (`claude --bg`, `claude agents`) | `aulas/segundo-plano/` |
| 4 | A sessêÂ£o gestora: ela coordena, vocêÂª decide | `aulas/sessao-gestora/` |
| 5 | Local, segundo plano ou nuvem (Projects) | `aulas/nuvem/` |
| 6 | Artifacts: do resultado ao link | `aulas/artifacts/` |
| 7 | Custo e controle | `aulas/custo/` |
| 8 | Seu sistema de gestêÂ£o de agentes | `aulas/sistema/` |

Cada aula tem um explicavideo com o avatar do Nei (canal ARCKHê, lives7).

## O processo, do inêÂ­cio ao fim

Legenda: ê°Å¸Â§Â  sessêÂ£o com o Nei êÂ· ê¢Å¡â¢ê¯Â¸Â script/timer êÂ· ê°Å¸Â¤â `claude -p` / subagente

1. ê°Å¸Â§Â  Pedido do Nei + conteêÂºdo de origem ê¢â â fatos conferidos na documentaêÂ§êÂ£o oficial (`longrun/2026-10-28-claude-gestor-agentes/FATOS.md` no repo wifi).
2. ê¢Å¡â¢ê¯Â¸Â Criar o curso: `~/.claude/skills/formato-curso-v72/scripts/novo-curso.sh ~/projetos/claude-gestor-de-agentes-v72 "Claude como gestor de agentes"`.
3. ê°Å¸Â¤â Escrever as aulas em `conteudo/pt/aulas/*.json` (um redator por par de aulas, sêÂ³ com fatos do FATOS.md).
4. ê°Å¸Â¤â Imagens: capa e fotos de abertura pelo Codex (`codex exec`, image_gen na assinatura) ê¢â â `assets/img/`.
5. ê¢Å¡â¢ê¯Â¸Â PortêÂ£o: `python3 gerar.py && python3 validar.py --links && node ~/.claude/skills/formato-curso-v72/scripts/conferir-tela.cjs .`
6. ê°Å¸Â¤â Revisor independente (agente novo, persona do pêÂºblico) ê¢â â corrigir ê¢â â revisar de novo; notas em `~/projetos/wifi/scripts/revisor-nota.py`.
7. ê¢Å¡â¢ê¯Â¸Â Publicar: commit + `gh repo create linnoff88-dev/claude-gestor-de-agentes-v72 --public --source . --push` + GitHub Pages da raiz.
8. ê°Å¸Â¤â Explicavideos: roteiro, visual e capa por aula (`~/projetos/output/claude-gestor-agentes-videos/cga-aN/`).
9. ê¢Å¡â¢ê¯Â¸Â Avatar no estêÂºdio HeyGen + render: `tools/lote.sh cga-aN ê¢â¬Â¦` (longrun) ê¢â â `entrega/cga-aN.mp4`.
10. ê¢Å¡â¢ê¯Â¸Â YouTube lives7 + bot v3 + ARCKHêytbot: `tools/plano16.sh` (dry-run) ê¢â â `tools/publica16.sh` (ou `tools/auto.sh`).
11. ê¢Å¡â¢ê¯Â¸Â VêÂ­deos no curso: release `video-v1.0.0` + `tools/embute.py` ê¢â â `gerar.py` ê¢â â push.
12. ê¢Å¡â¢ê¯Â¸Â Portal: skill `atualiza-portal` (curso em `courses.ts` + trilha Agentes Jarvis + enrichment) e vêÂ­deos em `videoUpdatesData`.
13. ê°Å¸Â§Â  r7ex 9:16 da novidade: `~/projetos/r7ex/edicoes/2026-10-28-claude-gestor-agentes/` ê¢â â `producao/producao.py --add` ê¢â â fila do lives7.
14. ê°Å¸Â§Â  Telegram ARCKHê.CCODE (skill `postar-telegram`) + MENU.

## Mais no ARCKHê AI
- [Ficha completa deste curso](https://www.ARCKHê AI/cursos/388-claude-como-gestor-de-agentes-saia-do-chat-e-coordene-uma-equipe-de-agentes/)
- [Guia: como aprender inteligêÂªncia artificial](https://www.ARCKHê AI/aprender-inteligencia-artificial/)
- [Todos os cursos](https://www.ARCKHê AI/cursos/)

ConteêÂºdo aberto e gratuito êÂ· formato ARCKHê Learning v7.2 êÂ· ARCKHê AI

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>