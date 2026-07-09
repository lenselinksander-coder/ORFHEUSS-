# ORFHEUSS Repository Status Model

Purpose: make every related repository readable before it becomes input for AI, Replit, Codex or governance work.

## Status fields

Each repository should carry an `ORFHEUSS_REPO_STATUS.md` file with these fields:

```text
ORFHEUSS layer:
Repository role:
Current status:
Source of truth:
May be used by AI as:
Must not be used as:
Missing dossiers:
Next action:
```

## Layer definitions

### CANON
Public preamble, constitutional framing, language, definitions, ontology and identity.

### KERNEL
Executable governance logic: gates, invariants, hard stops, audit rules, deterministic checks.

### APP
A user-facing application, prototype or runtime surface. Apps may contain prompts and interfaces, but they are not automatically canon.

### LESSON
Educational transfer layer: modules, curriculum, didactic framing, exercises and teacher material.

### ARCHIVE
Cultural, family, narrative, historical or source material. Archive is source, not runtime.

### ASSET
Supporting files, screenshots, generated images, attachments, exports and media.

### EXPERIMENT
Unstable proof of concept. May inspire, but may not be treated as source of truth.

### DEPRECATED
Historical material retained for reference. May not guide current builds unless explicitly revived.

## AI use rule

AI may use a repository only according to its status label.

- `CANON` may guide language and principles.
- `KERNEL` may guide technical governance logic.
- `APP` may guide interface and workflow only after dossier completion.
- `LESSON` may guide education and transfer.
- `ARCHIVE` may inform narrative context but must not be converted into live governance rules without human validation.
- `EXPERIMENT` may not be treated as stable architecture.

## Replit sync rule

When a Replit project is connected, add a missing dossier before treating the repository as complete:

```text
REPLIT_SOURCE.md
APP_DOSSIER.md
RUNTIME.md
DATA_MODEL.md
GOVERNANCE_BOUNDARIES.md
```

These documents define what the app does, how it runs, what data it handles, and which boundaries apply.
