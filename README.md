# paf-claude-skills

Skills pessoais do PAF (Paulo Ferreira) para Claude Code.

## Instalação (Claude Code marketplace)

```bash
/plugin marketplace add pafferreira/paf-claude-skills
/plugin install estilo-paf@paf-skills
/reload-plugins
```

## Instalação manual (sem marketplace)

```bash
git clone https://github.com/pafferreira/paf-claude-skills.git
cp -r paf-claude-skills/skills/estilo_paf ~/.claude/skills/
```

Reinicie o Claude Code. A skill aparece em `/help` como `estilo_paf`.

## Skills inclusas

### `estilo_paf` (v2.0.0)
Design system pessoal — paleta azul corporativa (#034EA2 / #008ACF), tipografia Nunito+Inter, componentes React/TSX padronizados, dark mode obrigatório, animações sem reflow, breakpoints mobile-first, z-index hierarchy, modais acessíveis, toasts, skeletons, empty states.

**Quando dispara:** qualquer tarefa de UI, CSS, componentes ou layout em projetos do PAF.

## Estrutura

```
paf-claude-skills/
├── .claude-plugin/
│   └── marketplace.json          # Catálogo do marketplace
├── plugins/
│   └── estilo-paf/
│       ├── .claude-plugin/
│       │   └── plugin.json       # Metadata do plugin
│       └── skills/
│           └── SKILL.md          # Skill empacotada
└── skills/
    └── estilo_paf/
        └── SKILL.md              # Skill standalone (instalação manual)
```

## Licença

MIT
