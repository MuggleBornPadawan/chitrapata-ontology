# Chitrapata Ontology

Single source of truth for the **Chitrapata** atelier and **Chittu 13.14** platform.

- `chitrapata.org` — canonical knowledge graph: atelier specs, license topology, PCG invariants, art series, compliance matrix.
- Audience: LLMs and coding agents (non-human). Zero hallucination tolerance. See file header.

## Use in a repo

Add as submodule (convention: `atelier/` path):

```bash
git submodule add https://github.com/MuggleBornPadawan/chitrapata-ontology.git atelier
```

Read from `atelier/chitrapata.org`. Update with:

```bash
git submodule update --remote atelier
```

## Edit rule

- Never edit a submodule copy inside a consumer repo.
- Change this repo, push, then update submodules downstream.

## Agent memory

Global `AGENTS.md` (opencode + pi) points here:

```text
Atelier Ground Truth (Chitrapata / Chittu 13.14)
- Canonical ontology: `<repo>/atelier/chitrapata.org` when present (submodule → `MuggleBornPadawan/chitrapata-ontology`)
- Upstream: https://github.com/MuggleBornPadawan/chitrapata-ontology
```

## License

GNU GPLv3 with EPL Section 7 Linking Exception. See `chitrapata.org` §§4.1–4.2.
