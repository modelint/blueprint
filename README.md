# Blueprint

The Blueprint toolchain is not yet another monolithic licensed MBSE (Model Based
Systems/Software Engineering) IDE.

Blueprint is a flexible, AI-ready, open source toolchain that you can use
alongside your existing MBSE tools and standards. Or use it entirely on its own.

You can use this toolchain to develop, execute, debug and test fully executable,
platform independent models.

And unlike most system modeling tools, Blueprint focuses on specifying the most
critical part of your system, especially when it comes to safety: the software.

While hardware specification is also critical, the required logic, behavior,
semantics, edge case detection and how it is all organized in your complex safety
critical system will make or break that system, regardless of the quality of the
hardware design.

My name is Leon Starr and I have been helping Fortune 500 teams build models of
mission safety critical systems for over 25 years. I got tired of watching
software developers using serious, powerful development environments while my
teams waste time pushing pixels and hopping around endless menu hierarchies and
struggle with crappy configuration management, limited license keys and many
other impediments to just getting the real work done. And I've seen many teams
abandon modeling altogether just because their MBSE tools never lived up to their
promise.

I designed Blueprint so I could focus on the analysis and modeling work that
solves the hard problems and makes a real difference on a project. I wanted to
work like a serious developer, get a system's software specified and delivered
and stop wasting time and effort on unproductive, busy-work modeling activities.

And now a primary focus is the integration of AI both as a source and a target of
MBSE development.

I now have enough of the toolchain built that I am ready to invite you to take a
look. Feel free to contact me if your team is interested in taking this kind of
approach on your MBSE (or currently non-MBSE) project.

— Leon Starr / leon_starr@modelint.com

## Why use Blueprint?

### Snap together building blocks

Use small modules that snap together with a human readable text pipeline.

So you can swap in your own modules, adapters, converters, etc.

Don't like one of the modules? Fork (modify) it or swap in your own.

Example modules: Diagram generator, action language parser, model execution
platform, model debugger, scenario populator.

### Generate whatever kinds of diagrams you want

Graphics are never embedded in the models themselves where the critical rules,
logic, behavior of your system are expressed. So changes to the graphical
presentation (intentional or accidental) won't affect the models themselves.

This separation gives you the power to view a model or any intermediate data in
the pipeline as a diagram using whatever notation and geometric layout you need.

The flatland and sequins diagram generator modules, for example, let you do
things like add annotation layers, highlight key model threads using a coloring
system to distinguish nominal, recoverable, and unrecoverable states, and
incorporate professional title blocks (like a blueprint).

### Real configuration management

Diagrams are always derived from human readable text, so just use your favorite
configuration management system.

- Was there a change to the models? Or just the layout? (or both?)
- Trash the layout? Rearrange your diagrams? Models themselves are unaffected.

### Executable at ALL levels

The models are not just vacuous box-in-box hierarchies.

The data, logic, behavior, AND actions (computation) are all modeled with full
executability without the need for any programming language components.

The action language lets you specify fully detailed platform independent
computations without having to insert code to make it work.

### Compatibility with standards (SysML V2, UML) or proprietary tooling

Since the models are text and they use semantics defined by existing standards,
they can be converted or represented with whatever standards compliant formats
you need. This includes proprietary tool standards.

### Use your existing development tools

You should be able to develop, view, debug, test and deploy MBSE models with your
existing development tools just like any software project.

Models are expressed and maintained as human readable text.

Use your favorite text editor, IDE, configuration management, and AI tools to
develop and manage your models.

### Diagrams are generated exactly the way you want them

No more fighting with a layout algorithm or AI to produce exactly what you want.
No more pushing pixels by hand (or even specifying pixels).
You control the layout with flexible diagramming semantics that AI can understand.

### No GUI — yes, that's a feature

I've seen teams waste endless time pushing pixels and dragging and dropping and
bouncing around in hierarchies of endless menus.

Sometimes the best GUI is your text editor.

You can get everything done in Blueprint using your favorite text editor, possibly
in your favorite IDE. I typically use PyCharm and Claude Code to get my modeling
work done.

And that's one of the reasons why Blueprint can be used on so many development
platforms.

And that's another reason why you don't have to worry about any critical data
being locked up in the tool and why you don't need a license key to access your
models.

That said, there's nothing stopping you from creating a nice GUI front end to one
or more Blueprint modules.

### Platform independent modeling

Blueprint supports a modeling methodology that completely separates
platform/design/implementation details from essential system rules, logic, and
behavior.

So critical safe behavior can be implemented and certified across multiple system
versions or deployments.

And your models remain stable while the target platform evolves.

### Domain driven development

The supported methodology also emphasises platform independent domain separation.

This ensures that complex systems scale and are highly configurable.

### Executable models

No more 'concept of a plan' modeling. Blueprint models execute so you can test
them objectively, just like code.

### Fully open source (MIT license)

All the tools are freely available with no features restricted.

License and purchase of integrations or proprietary extensions and services are
available.

## The tools

Blueprint is documentation only in this repository — the individual tools live in
their own repositories under the [`modelint`](https://github.com/modelint)
organization.

📖 **[Read the docs in the Blueprint wiki](https://github.com/modelint/blueprint/wiki)** —
how the tools fit together, plus a page for each tool.

| Tool | Repository | Role |
|------|------------|------|
| Flatland | [flatland](https://github.com/modelint/flatland) | Model + layout text → diagram |
| xuml-populate | [xuml-populate](https://github.com/modelint/xuml-populate) | Populate a model into the xUML metamodel repository |
| make-xuml-repo | [make-xuml-repo](https://github.com/modelint/make-xuml-repo) | Build the model repository database from the metamodel |
| mx | _(add repo)_ | _(describe)_ |
| mdb | [model-debugger](https://github.com/modelint/model-debugger) | Modeling-language-independent model debugger |