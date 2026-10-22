# Skills del Taller de Claude

Skills por rol para el Taller de Claude (Venezuela).

| Plugin | Skills | Para |
|---|---|---|
| taller-abogados | triage-nda-venezuela | Abogados |
| taller-contadores | estados-financieros-venezuela | Contadores |
| marketing (de Anthropic) | brand-review, campaign-plan, draft-content y más | Marketing |

Gerencia usa la skill de Excel (xlsx), que ya viene incluida en Claude.

## Instalar (Claude web o escritorio, plan pago)

1. Personalizar › Plugins › Agregar › Agregar marketplace › Agregar desde un repositorio.
2. Pegar: `alejandrofaraco982-glitch/skills-taller-claude`
3. Agregar el plugin de tu rol.

## Instalar (Claude Code)

```
/plugin marketplace add alejandrofaraco982-glitch/skills-taller-claude
/plugin install taller-abogados@taller-claude
/plugin install taller-contadores@taller-claude
/plugin install marketing@taller-claude
```

Las skills adaptadas a Venezuela son un filtro inicial y no sustituyen a un abogado o a un contador público colegiado.
