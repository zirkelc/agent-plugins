# claude-plugins

Claude Code plugins by [Chris Cook](https://github.com/zirkelc). Add the marketplace once,
install whichever ones you want.

```
/plugin marketplace add zirkelc/agent-plugins
```

| plugin | |
|---|---|
| [agent-journal](https://github.com/zirkelc/agent-journal) | A journal written by your agent, autonomously. One small markdown file per milestone, written as the work happens, in a format built to be scanned with grep and ls. |
| [agent-history](https://github.com/zirkelc/agent-history) | Exports every Claude Code session and its subagents to a folder as JSONL and Markdown, and commits and pushes it when the folder is a git repository. |
| [quick-actions](https://github.com/zirkelc/claude-quick-actions) | A band above the prompt with buttons that run saved prompts, skills and shell commands. |
| [git](https://github.com/zirkelc/claude-git) | Git status above the prompt and a source control panel: changes, commit, history graph, branches and worktrees, one-click sync, and how far the branch is behind its base with a merge preview. |

```
/plugin install agent-journal@zirkelc
/plugin install agent-history@zirkelc
/plugin install quick-actions@zirkelc
/plugin install git@zirkelc
```

The operands read `<plugin>@<marketplace>`, so the marketplace name comes second.

## What is in here

Only this marketplace manifest. Each plugin lives in its own repository, with its own
README, issues, and releases, and this repo points at them. Nothing is vendored, so
installing takes whatever is on the plugin's default branch.

Adding a plugin means one entry in `.claude-plugin/marketplace.json`. Entries deliberately
carry no `version`: the plugin's own `plugin.json` is the only place a version is declared,
so there is nothing here to drift out of date.
