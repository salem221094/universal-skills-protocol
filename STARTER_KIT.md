# ASP v2.0 Starter Kit 🛠️

This starter kit provides the essential tools to build, validate, and maintain **Advanced Skills Protocol (ASP) v2.0** compliant skills.

## 📦 Included Scripts

### 1. `skill_factory.py` (The Scaffolder)
Use this to generate new skills with the mandatory ASP skeleton.
```bash
python3 scripts/skill_factory.py --name "my-new-skill" --desc "A brief description"
```

### 2. `repair_skills.py` (The Validator)
Run this to audit your skills directory and automatically fix structural drift.
```bash
python3 scripts/repair_skills.py --dir ./skills --fix
```

## 🛡️ ASP Compliance Badge
Add this to your repository's README to show you follow the standard:

```markdown
[![ASP v2.0 Compliant](https://img.shields.io/badge/ASP-v2.0_Compliant-blueviolet)](https://github.com/salem221094/universal-skills-protocol)
```

## 🚀 Getting Started

1.  **Clone this repo**: `git clone https://github.com/salem221094/universal-skills-protocol`
2.  **Move tools to your project**: Copy the `scripts/` folder to your agentic project.
3.  **Standardize your instructions**: Run the repairer against your existing prompt files.
