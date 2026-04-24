---
description: How to contribute to the RogueBlade wiki.
---

# 🤝 Contributing

This wiki lives on [GitHub](https://github.com/Serokai/rogueblade-wiki) and syncs to GitBook. Anyone can contribute.

## Quick workflow

1. Fork the repository
2. Edit the relevant `.md` file (see `SUMMARY.md` for the structure)
3. Open a pull request with a [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) message

## Commit style

| Prefix | Use for |
|---|---|
| `feat:` | A new page or section |
| `docs:` | Content additions/changes on an existing page **(most common here)** |
| `fix:` | Correcting wrong info, broken links |
| `chore:` | Config, tooling, `.gitbook.yaml` |
| `refactor:` | Restructuring without content change |

Example: `docs(classes/vampire): add skill descriptions and mastery details`

## Style guide

{% hint style="success" %}
Every page starts with a `description:` front-matter block. GitBook renders it as the page subtitle and uses it for search previews — **keep it meaningful**.
{% endhint %}

* Use `{% hint %}` blocks for tips, warnings and callouts (`info`, `success`, `warning`, `danger`)
* Keep emojis consistent with those used in `SUMMARY.md`
* Link generously between pages — cross-references are what make a wiki useful
* Numbers and mechanics go **stale fast**. Always tag which patch you sourced the info from when writing balance details

## Useful GitBook snippets

**Cards**

```
<table data-view="cards">
  <thead><tr><th></th><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead>
  <tbody>
    <tr><td><strong>Title</strong></td><td>Description</td><td><a href="page.md">page.md</a></td></tr>
  </tbody>
</table>
```

**Tabs**

```
{% tabs %}
{% tab title="Normal" %}
Content here.
{% endtab %}
{% tab title="Nightmare" %}
Content here.
{% endtab %}
{% endtabs %}
```
