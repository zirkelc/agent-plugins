# claude-plugins

Claude Code plugins by [Chris Cook](https://github.com/zirkelc). Add the marketplace once,
install whichever ones you want.

```
/plugin marketplace add zirkelc/claude-plugins
```

| plugin | |
|---|---|
| [agent-reminders](https://github.com/zirkelc/agent-reminders) | Reminders that survive the session that created them. One markdown file each, carrying its own context, surfaced at session start in the project it belongs to. |

```
/plugin install agent-reminders@claude-plugins
```

The operands read `<plugin>@<marketplace>`, so the marketplace name comes second.

## What is in here

Only this marketplace manifest. Each plugin lives in its own repository, with its own
README, issues, and releases, and this repo points at them. Nothing is vendored, so
installing takes whatever is on the plugin's default branch.

Adding a plugin means one entry in `.claude-plugin/marketplace.json`. Entries deliberately
carry no `version`: the plugin's own `plugin.json` is the only place a version is declared,
so there is nothing here to drift out of date.
