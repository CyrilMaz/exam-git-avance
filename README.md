# Campus Library — Examen Git

# Ce repository contient plusieurs branches avec du code pré-écrit.

# comment éxécuter le code

Prérequis :
- Avoir Go installé (v1.18+). Vérifier avec `go version`.
- Travailler depuis le répertoire racine du projet (contenant `go.mod`).

Exécution (développement)
Ouvrir PowerShell dans le dossier du projet puis exécuter :

```powershell
go run .
# ou
go run main.go
```

Le serveur démarre sur `http://localhost:8080`.

Routes principales :
- `/` : page d'accueil (liste des livres)
- `/book?id=1` : page détail du livre (remplacer `1` par l'ID)
- `/contact` : page de contact

Compiler un exécutable (Windows PowerShell) :

```powershell
go build -o campus-library.exe
.\campus-library.exe
```

Remarques :
- Lancer les commandes depuis le répertoire racine pour que les templates et assets soient trouvés.
- Pour changer le port, modifier `main.go` (ligne `ListenAndServe(":8080", ...)`).

# participants
Cyril Mazauric



# Arborescence actuelle #

├── go.mod
├── main.go
├── .gitignore        // précise que go.mod doit être ignoré par git
├── data
│   └── books.go      // liste des livres
│
├── handlers
│   └── books.go      // Handlers : liste + détail         
│
├── templates        
│   ├── book.html     // Page d’un livre (route dynamique)         
│   ├── contact.html  // Page des contacts         
│   └── home.html     // Page d'accueil        
│
├── static
│   └── style.css
│
└── README.md