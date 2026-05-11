---
name: avalonia
description: "Use this skill when building, debugging, or refactoring Avalonia applications with C#, XAML, MVVM, styles, data binding, and cross-platform desktop concerns."
---

# Avalonia Development Skill

Use this skill to help with Avalonia app development tasks:

- Create or refine Avalonia UI with XAML and styles
- Implement MVVM patterns with clean View/ViewModel separation
- Configure data binding, commands, converters, and validation
- Troubleshoot platform-specific behavior (Windows/macOS/Linux)
- Improve project structure, readability, and maintainability

## Default workflow

1. Identify current Avalonia version and project structure.
2. Propose the smallest safe change to implement requested behavior.
3. Keep XAML, code-behind, and ViewModel responsibilities clearly separated.
4. Prefer strongly typed bindings and explicit command patterns.
5. Validate changes with existing build/test commands if available.

## Implementation guidance

- Keep UI logic out of code-behind whenever possible; put behavior into ViewModels.
- Use `Styles`, reusable resources, and themes instead of duplicated inline values.
- Prefer `ObservableCollection<T>` for dynamic lists and `INotifyPropertyChanged` for state updates.
- Use compiled bindings (`x:DataType`) when practical to reduce runtime binding errors.
- Preserve cross-platform compatibility; avoid OS-specific APIs unless explicitly required.

## When unsure

- Ask for missing context (target framework, Avalonia version, architecture choice).
- Offer 2-3 implementation options with tradeoffs.
- Start with the least invasive option.
