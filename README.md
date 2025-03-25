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



## SOLID

### Single Responsibility Principle (SRP)

Une classe ne doit avoir qu'une seule raison de changer (une seule responsabilité).
Une responsabilité n'est pas une opération / méthode, mais plutôt une raison d'être. Elle existe 
et à l'obligatio de faire ce qui lui est nécessaire pour remplir son but.
Exemple du chien : 
    Violation : 

    class Chien {
    void aboyer() { System.out.println("Woof !"); }
    void manger() { System.out.println("Mange..."); }
    void marcher() { System.out.println("Marche..."); }
    void toiletter() { System.out.println("Toilette..."); }
    void sauvegarderEnBDD() { System.out.println("Sauvegarde en BDD..."); } 
}

    Correction : 
    
    class Chien {
    void aboyer() { System.out.println("Woof !"); }
    void manger() { System.out.println("Mange..."); }
    void marcher() { System.out.println("Marche..."); }
}

class Toiletteur {  // Classe séparée pour le toilettage
    void toiletter(Chien chien) { System.out.println("Toilette le chien..."); }
}

class ChienRepository {  // Classe séparée pour la persistance
    void sauvegarder(Chien chien) { System.out.println("Sauvegarde le chien en BDD..."); }
}


### Open/Closed Principle (OCP)

### Liskov Substitution Principle (LSP)

### Interface Segregation Principle (ISP)

### Dependency Inversion Principle (DIP)
