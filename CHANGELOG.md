# Changelog

## 1.0.2 - 2026-11-16

Launch price: premium pack $29 to $15. The pack itself is unchanged.

## 1.0.1 - 2026-11-16

Test fixes, from the agent test run:

- The validator now fails a file that still contains the documented placeholder attachment ID 12345 or a placeholder example.com image URL, instead of only warning about it. A file with a placeholder is not ready to import.
- SKILL.md troubleshooting: the `classes: invalid_value` row now covers a dangling class reference, not only a regenerated style ID.
- SKILL.md: new-project fallback for constants (state the constants you chose in the delivery note) and a note that exported files usually carry desktop and mobile variants only, so the validator does not check tablet variants.

## 1.0.0 - 2026-11-16

First release.

- Free skill: the five hard rules, the build rules, the delivery rules, a worked transplant example, and a troubleshooting table.
- Example hero section skeleton in valid Elementor JSON.
- Transplant checklist.
- Premium pack: `validate.py` pre-import checker, five reference patterns, canonical envelopes, import QA checklist.
