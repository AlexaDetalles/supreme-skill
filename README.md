<p align="center"><img src="docs/banner.svg" alt="SUPREME — Del objetivo a la evidencia." width="100%"></p>

<p align="center"><strong>Workflow proporcional para planificar, implementar y verificar tareas completas.</strong><br>Una skill portable, recursos bajo demanda y resultados verificables.</p>

<p align="center">Claude Code · Codex · Agent Skills · MIT</p>

## Qué hace

Define aceptación · Elige una ruta · Implementa · Verifica · Entrega.

## Instalar en Claude Code

En Claude Code:

```text
/plugin marketplace add AlexaDetalles/supreme-skill
/plugin install supreme@supreme-skills
```

Invocar la skill del plugin con `/supreme:supreme`. También puedes copiar solamente `skills/supreme/` a `~/.claude/skills/supreme/` para usar `/supreme` sin plugin.

## Instalar en Codex

Desde una carpeta de trabajo, clona el repositorio y copia la skill al directorio de skills personales. Ejemplo PowerShell:

```powershell
git clone https://github.com/AlexaDetalles/supreme-skill.git
New-Item -ItemType Directory -Force "$HOME/.agents/skills" | Out-Null
Copy-Item -Recurse "./supreme-skill/skills/supreme" "$HOME/.agents/skills/supreme"
```

Si ya existe una instalación, revísala o respáldala antes de reemplazarla. Usa `$supreme` en Codex. En versiones que utilicen otra carpeta de skills, copia el mismo directorio al destino configurado por tu instalación.

## Un ejemplo

```text
Corrige este bug: reproduce el fallo, aplica el cambio mínimo y verifica el comportamiento.
```

## Qué contiene

| Ruta | Propósito |
|---|---|
| `skills/supreme/SKILL.md` | Instrucciones portables |
| `skills/supreme/agents/openai.yaml` | Metadatos de Codex |
| `.claude-plugin/` | Plugin y catálogo para Claude Code |
| `LICENSE` y `NOTICE.md` | Condiciones y procedencia |
| `docs/` | Identidad visual del repositorio |

## Requisitos y límites

Sin dependencias de ejecución. Las herramientas concretas dependen de la tarea; el workflow no instala plugins ni transforma el modelo.

La compatibilidad estructural se comprueba localmente; la carga real debe verificarse en cada cliente. No se promete acceso a herramientas ausentes, ahorro medido de tokens ni resultados infalibles.

## Contribuir

Consulta [CONTRIBUTING.md](CONTRIBUTING.md). Para información sensible, consulta [SECURITY.md](SECURITY.md).

## Licencia y créditos

MIT para las aportaciones originales de Isaac / KROMBYTE. Consulta [NOTICE.md](NOTICE.md) para procedencia y condiciones de material externo. Proyecto independiente, sin afiliación con Anthropic u OpenAI.
