# Symbolic Function vs Visual Form

## Purpose

This file explains the distinction between what a motif looks like and what it may mean — and why this distinction is critical throughout the repository.

---

## The core distinction

**Visual form** is what the motif looks like:
- its shape, geometry, contour
- its symmetry type
- its repeat behavior
- its compositional role (border, field, emblem, scene element)
- its abstraction level
- its line quality (angular, curvilinear, mixed)

**Symbolic function** is what the motif may represent or do:
- protection, guardianship
- fertility, renewal
- royal authority, divine status
- cosmological order
- passage between states or worlds
- clan or group identity

---

## Why the separation matters

Motifs that look similar across traditions often carry different symbolic weight.

### Example: spirals

- In some Polynesian traditions, spiral forms relate to growth, genealogy, and ocean movement.
- In some Celtic contexts, spirals appear on megalithic monuments; their symbolic reading is debated and largely speculative.
- In Greek ornament, the spiral functions primarily as a border meander — a compositional device, not necessarily a symbol.

Treating all spirals as "meaning the same thing" is a collapse of specificity.

### Example: rosette forms

- In Mesopotamian art, rosette forms appear on palace reliefs and cylinder seals. They are often associated with divine figures but their precise meaning is context-dependent.
- In European folk art, rosette forms appear in carved wood and painted furniture. Their symbolic reading is often thin or uncertain.
- In Islamic geometric ornament, rosette-like forms emerge from tessellation logic and may not carry the same emblematic role as in other traditions.

The same visual form can serve different compositional and symbolic purposes.

---

## Practical implications

### For prompting
Specifying a motif by form ("eight-pointed star tessellation") is more reliable than specifying by meaning ("symbol of cosmic order"). Meaning-based prompts tend to produce generic, drifted outputs.

### For generative systems
Generative systems can reproduce visual form more reliably than symbolic content. The repo should provide formal descriptions that systems can act on, with symbolic notes as context — not as the primary instruction.

### For retrieval and tagging
Tags should include both formal and symbolic dimensions, but formal tags should be primary. A rosette is retrievable by shape. Its symbolic role depends on which tradition it comes from.

---

## When symbolic claims are appropriate

Symbolic claims are appropriate when:

- the tradition has documented symbolic conventions (e.g., Egyptian hieroglyphic context, Hindu iconographic programs)
- the interpretation is supported by material evidence or established scholarship
- the claim is qualified by context, period, and medium

Symbolic claims should be reduced or omitted when:

- the motif's meaning is speculative
- the interpretation relies mainly on modern projection
- the motif functions primarily as a compositional element

---

## Default behavior

When in doubt:
- describe the form
- note the compositional role
- mention symbolic tendencies only if grounded
- flag uncertainty explicitly
