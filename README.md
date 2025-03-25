# Notes


## Clean Code

### Commit

#### Model : 

type(scope): subject

body

footer



type: Décris la raison du commit (ex.: feat, fix, docs).

scope: (optionnel): Specifie la partie du codebase affectée (ex.: auth, navbar, config).

subject: Sommaire concis des changements

body: (optionnel): Description détaillée des changements.

footer: (optionnel): Référence (e.g., Closes #123) ou changement qui brisent quelque chose.

#### Types
feat:	A new feature (triggers a minor version bump in SemVer).
fix:	A bug fix (triggers a patch version bump in SemVer).
docs:	Documentation changes (e.g., README, comments).
style:	Formatting, whitespace, or non-functional changes (e.g., linting).
refactor:	Code restructuring without fixing bugs or adding features.
perf:	Performance-related improvements.
test:	Adding or modifying tests.
chore:	Maintenance tasks (e.g., dependency updates, CI/CD changes).
build:	Build system or external dependency changes (e.g., Webpack, npm).
ci:	CI/CD pipeline changes (e.g., GitHub Actions, Jenkins).
revert:	Reverts a previous commit.



