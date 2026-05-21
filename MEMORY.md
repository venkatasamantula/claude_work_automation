# Memory Protocol

## Rule for every session
1. **Before doing any work**, read `thoughtStarter/memory/interaction.md` to recover prior context, user preferences, and past thought starters. Do this silently — don't ask the user to repeat anything that's already logged.
2. **After completing each interaction**, append a new dated entry to `thoughtStarter/memory/interaction.md` capturing:
   - The thought starter (or other request)
   - Decisions and preferences observed
   - Output file(s) produced
   - Anything the user pushed back on or asked to change
3. **Never overwrite** prior entries in `interaction.md`. Always append.
4. Individual generated posts continue to be saved as their own timestamped `.txt` files in `thoughtStarter/memory/` (per the ThoughtLeader agent spec). The `interaction.md` log indexes and contextualizes them.

## Pointers
- Agent definitions: `thoughtStarter/agents/`
- Prompt templates: `thoughtStarter/prompts/`
- Generated posts + interaction log: `thoughtStarter/memory/`
- Project overview: `CLAUDE.md`
