# claude-hunch: Claude Code in hunch

A Claude Code plugin that makes Claude a participant in hunch 0.1.0:

- While an editor is registered, Claude's own edits to the human's files
  are denied. Claude makes them through the editor or in a git worktree,
  as the hunch skill says.
- Claude registers as `agent` for the length of a session, so others can
  find it, e.g. tmux-hunch sends it pastes from the editor.

## Install

Needs `hunch` and `hunch-editor` on PATH, `jq`, and the hunch skill in
`~/.claude/skills`. In Claude Code:

    /plugin install hunch --marketplace roolebo/claude-hunch
