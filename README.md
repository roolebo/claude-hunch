# claude-tribe: Claude Code in tribe

A Claude Code plugin that makes Claude a participant in tribe 0.1.0:

- While an editor is registered, Claude's own edits to the human's files
  are denied. Claude makes them through the editor or in a git worktree,
  as the tribe skill says.
- Claude registers as `agent` for the length of a session, so others can
  find it, e.g. tmux-tribe sends it pastes from the editor.

## Install

Needs `tribe` and `tribe-editor` on PATH, `jq`, and the tribe skill in
`~/.claude/skills`. In Claude Code:

    /plugin install tribe --marketplace roolebo/claude-tribe
