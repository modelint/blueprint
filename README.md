# Blueprint

An overview of the **Blueprint** modeling-tool ecosystem: the set of tools that
together take a Shlaer-Mellor Executable UML (xUML) model from text and layout
files through to a populated metamodel repository, diagrams, and execution.

This repository is documentation only — there is no application code here. The
individual tools live in their own repositories under the
[`modelint`](https://github.com/modelint) organization.

## 📖 Read the docs in the [Blueprint wiki](https://github.com/modelint/blueprint/wiki)

The wiki is the detailed write-up: how the tools fit together, plus a page for
each tool.

## The tools

| Tool | Repository | Role |
|------|------------|------|
| Flatland | [flatland](https://github.com/modelint/flatland) | Model + layout text → diagram |
| xuml-populate | [xuml-populate](https://github.com/modelint/xuml-populate) | Populate a model into the xUML metamodel repository |
| make-xuml-repo | [make-xuml-repo](https://github.com/modelint/make-xuml-repo) | Build the model repository database from the metamodel |
| mx | _(add repo)_ | _(describe)_ |
| mdb | [model-debugger](https://github.com/modelint/model-debugger) | Modeling-language-independent model debugger |