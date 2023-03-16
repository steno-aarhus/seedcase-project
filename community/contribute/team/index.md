---
title: How we work
---

{{< include /includes/_wip.qmd >}}

## Communication across team and collaborators

Our general philosophy is to limit meetings and emails as much as is
appropriate, and instead use text-based forms of communication. For
shorter or quick questions, we use our Discord channel. For longer
discussions, we use GitHub Issues. And for help or sharing information,
we use blog posts that we add to the website.

No matter which communication channel is used, we write in Markdown
format, though Discord uses a limited set of Markdown features.

## Guide to the general workflow

-   When adding or modifying content on either the website or the
    product itself, we follow the "branch-pull request" workflow. This
    is described in more detail in the [GitHub
    Flow](https://docs.github.com/en/get-started/quickstart/github-flow)
    page.

There are some scripts to help automate some of the tasks of working on
the project. They are all found in the `src/` folder. All of them
require opening a Terminal, and how you do that depends on the
application you are using.

> If you don't know what any of this means, the Team Lead or another
> member will handle it.

::: panel-tabset
### RStudio

If you use RStudio, you can use the Command Palette
(`Ctrl/Cmd-Shift-P`), followed by typing "new terminal", and hit enter.
A new Terminal should open beside the Console (by default).

### VS Code

If you use VS Code, you can run this command by using `Ctrl/Cmd-Shift-P`
to access the Command Palette, then type out "terminal create new", and
finally hit enter. A Terminal will open up on the bottom, which is where
you can run the reformat markdown script.
:::

| Action                                               | Command                                  |
|------------------------------------------------------|------------------------------------------|
| Reformat Markdown to Pandoc canonical format         | `bash src/pr/reformat-markdown.sh`       |
| Run PlantUML on `.puml` files to re-build the images | `bash src/regenerate-plantuml-images.sh` |

: Scripts to help automate our work.

## Guide to admin tasks

-   With the Seedcase product, Git tags and releases are added fairly
    regularly. On the other hand, with the website, we only tag a
    version of the website after a major "milestone" or deadline. For
    instance, after sending the design documents to get reviewed or when
    sending an update document to our funder or stakeholders.

| Action            | Command              |
|-------------------|----------------------|
| Reformat Markdown | `/reformat_markdown` |

: Pull Request helpers