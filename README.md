# Campus Library — Examen Git

Ce repository contient plusieurs branches avec du code pré-écrit.

🎯 Votre objectif : reconstruire le projet final en utilisant **exclusivement Git** :
- fork
- pull requests
- merges
- résolution de conflits
- tags
- historique propre*



# Arborescence actuelle #
o│ = fait

 │ = à faire


o├── go.mod
 ├── go.sum
o├── main.go
 │
o├── data
 │   └── books.go      // Données simulées : liste des livres         
 │
o├── handlers
o│   └── books.go      // Handlers : liste + détail         
 │
 ├── templates
 │   ├── layout.html   // Layout global (header/footer)         
 │   ├── index.html    // Page d'accueil         
 │   ├── books.html    // Page listant tous les livres         
 │   └── book.html     // Page d’un livre (route dynamique)         
 │
o├── static
o│   └── style.css
o│
o└── README.md