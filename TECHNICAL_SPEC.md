# ASP v2.0 Technical Specification (Plug-and-Play)

This document defines the **Advanced Skills Protocol (ASP)**. Any system or IDE compliant with this spec can host, validate, and maintain high-fidelity AI Skills without human supervision.

## 1. File Structure (The Anatomy)
Every `SKILL.md` must follow this mandatory byte-order:

1.  **YAML Frontmatter**: 
    - Must start and end with `---`.
    - Must contain `name` and `description` keys.
2.  **Strategic Research Block**: 
    - Header: `## Step 0: Modern Technology Research (MANDATORY)`
    - Purpose: Forces the agent into a "retrieval-first" state.
3.  **Heuristic/Intelligence Block**:
    - The creative instruction layer (Free-form Markdown).
4.  **Validation Gate**:
    - Header: `## Definition of Done`
    - Logic: Must contain a list of GFM checkboxes (`- [ ]`).

## 2. Validation Logic (The Guard)
A compliant ASP Validator must iterate through the repository and verify:
- **Regex Check**: `^---[\s\S]+?---` (YAML verification).
- **String Check**: Existence of mandatory UTF-8 section headers.
- **Sanitization**: Absence of non-printable or illegal artifacts.

## 3. Deployment (Plug-and-Play)

### For IDEs (VS Code/Cursor):
- **Linting**: Add automated repair scripts to your pre-save hooks.
- **Scaffolding**: Use automated factories to generate new skills instead of `touch`.

### For Agents (Auto-GPT/Claude):
- **On-Load Protocol**: "Load ASP Specification. If a requested skill is non-compliant, run the Repairer before execution."

## 4. Reference Implementation
The canonical tools for this spec are found in the official ASP registries and supporting repositories like [MAD-Logic](https://github.com/salem221094/mad-logic).
