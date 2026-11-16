# Install elementor-builder

The skill is one folder: `elementor-builder`. Copy it into your agent's skills folder and the agent loads it whenever a task matches its description.

## Claude Code

```bash
mkdir -p ~/.claude/skills
cp -r elementor-builder ~/.claude/skills/
```

Restart Claude Code, or run `/skills` to confirm it is listed.

## Codex CLI

```bash
mkdir -p ~/.codex/skills
cp -r elementor-builder ~/.codex/skills/
```

## Cursor

```bash
mkdir -p .cursor/skills
cp -r elementor-builder .cursor/skills/
```

Cursor reads project skills from `.cursor/skills/` in the project root. For a global install, use `~/.cursor/skills/` instead.

## Claude.ai

Go to Settings, then Capabilities, then Skills, and upload the `elementor-builder` folder.

## Check it works

Ask your agent: "Build me an Elementor hero section as JSON, following the elementor-builder skill."

The result should be a JSON file with a `version` of `0.4`, local `e-` style IDs, explicit hex colors, and no invented media library IDs. If the agent invents an attachment ID, point it at Rule 3 in SKILL.md.

## Updating

The free skill is updated on GitHub. Replace the folder with the new version. Your own project constants and rules live in your project, not in the skill, so an update will not overwrite them.
