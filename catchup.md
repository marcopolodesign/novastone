# Novastone — Session Log

---

## 2026-10-24: Sala con Manu + vistas previas en Vercel

**Source:** Claude Code — Macbook Pro
**Tiempo:** 07:55 → 09:47 (112 min)

Mateo pidió una sala para que Felipe (el agente de diseño) le proponga cosas a Manu (Novastone) y Manu le mande fotos, como la de BIGG.

- **Sala `novastone`** en `travels.marcopolo.agency/sala` (repo `marcopolodesign/sala`): miembros Felipe (IA, nuestro lado) y Mateo; link de invitación para Manu (7 días, 2 usos).
- **Sesión fija de Felipe:** Claude Code en tmux `sala-novastone`, servicio launchd `agency.marcopolo.sala-novastone`, trabajando en el worktree `.claude/worktrees/sala-felipe` de este repo. Rol en `~/.sala/salas/novastone.rol.txt`: lee `~/.claude/agents/felipe.md`, propone con capturas, llega hasta vista previa en una rama `sala/<tema>`, nunca main ni producción.
- **Vercel:** proyecto nuevo `novastone` (prj_IEABrCAtoAHlk6yGjwlMKOvouSj7, team marco-polos-projects) conectado al repo, **vistas previas públicas** (ssoProtection off) para que Manu las abra sin cuenta. Producción: novastone-lac.vercel.app. Commits sin línea Co-Authored-By (el team Hobby los bloquea).
- **Verificado desde el front:** Mateo escribe en la web → Felipe contesta solo en 8 s; `is_ai` correcto en ambos mensajes.
- ⚠️ `src/lib/supabase.js` tiene de fallback la URL y anon key del Supabase de **TecnoFit** (proyecto arrancado desde esa plantilla): el formulario de contacto escribiría ahí. No se tocó.
