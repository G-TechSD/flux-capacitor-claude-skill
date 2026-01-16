# Claude Skills Collection

A collection of custom skills for [Claude Code](https://claude.com/claude-code) that extend its capabilities with specialized behaviors and workflows.

## What are Claude Skills?

Skills are custom commands and behaviors you can add to Claude Code. They're defined using markdown files with YAML frontmatter that tell Claude when and how to use them.

## Available Skills

### 🚀 FLUX - Flux Capacitor Wiggum Loop

**Never stop at "good enough" - iterate until time runs out!**

The FLUX skill implements continuous iteration and improvement. When you reach a "done" state, FLUX keeps going - refining, enhancing, and polishing until your specified time limit expires.

**Usage:**
```
/flux 1 hour - test the app for all use cases
/flux 2 days - build and refine the app based on the kickoff script
/flux 5 minutes - come up with 1000 unique cat facts
/flux 30 seconds - fix the typo in README
```

**Philosophy:**
- "Done" is just the beginning
- There's always room for improvement
- Aim for that "Great Scott!" reaction
- Go above and beyond expectations

[Read the full FLUX documentation →](flux/SKILL.md)

## Installation

### Personal Installation (All Projects on This Machine)

```bash
# Clone the repository
git clone https://github.com/G-TechSD/claude-skills.git

# Copy skills to your personal Claude directory
cp -r claude-skills/*/ ~/.claude/skills/

# Or use symlinks to stay synced with updates
ln -s $(pwd)/claude-skills/flux ~/.claude/skills/flux
```

### Project-Specific Installation

```bash
# From your project directory
mkdir -p .claude/skills

# Copy the skills you want
cp -r /path/to/claude-skills/flux .claude/skills/

# Commit to your repo so your team gets the skills too
git add .claude/skills/
git commit -m "Add Claude skills"
```

### Verify Installation

Start Claude Code and ask:
```
What skills are available?
```

You should see the installed skills in the list!

## Creating Your Own Skills

Skills are easy to create! Here's the basic structure:

```bash
mkdir -p ~/.claude/skills/my-skill
```

Create `~/.claude/skills/my-skill/SKILL.md`:

```yaml
---
name: my-skill
description: Brief description of what this skill does and when to use it
---

# My Skill

## Instructions
Clear step-by-step guidance for Claude to follow.

## Examples
Show concrete examples of using this skill.
```

That's it! Claude will automatically discover and use your skill.

## Contributing

Have a great skill idea? Contributions welcome!

1. Fork this repository
2. Create your skill in a new directory
3. Add documentation to this README
4. Submit a pull request

## Skill Ideas

Some ideas for future skills:
- **deep-review**: Multi-pass code review with security, performance, and architecture analysis
- **test-everything**: Comprehensive test generation (unit, integration, e2e)
- **document-master**: Generate thorough documentation from code
- **refactor-guru**: Systematic refactoring with best practices
- **debug-detective**: Methodical debugging workflow
- **performance-optimizer**: Profile and optimize systematically

## License

MIT License - feel free to use, modify, and share!

## Links

- [Claude Code Documentation](https://docs.anthropic.com/claude-code)
- [Skills Documentation](https://docs.anthropic.com/claude-code/skills)

---

*"Great Scott! These skills are heavy!"*
*"There's that word again, heavy. Why are things so heavy in the future? Is there a problem with the Earth's gravitational pull?"*
