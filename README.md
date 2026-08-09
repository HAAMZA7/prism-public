<div align="center">

# ◆ PRISM

### Plateforme GRC nouvelle génération.

Gouvernance, Risque et Conformité — conçue comme un produit, pensée pour l'entreprise.

</div>

---

PRISM centralise la gestion de la conformité, de l'analyse de risque et du pilotage des contrôles dans une interface moderne, sombre et minimale. L'objectif : faire de la GRC un outil utilisable au quotidien — pas un classeur de documents.

## Ce que fait la plateforme

- **Gouvernance** — pilotage central de la conformité, liens intelligents entre objets (normes, contrôles, actifs, risques)
- **Gestion des risques** — analyse et évaluation continues, suivi des plans de remédiation
- **Conformité multi-normes** — frameworks prêts à l'emploi (ISO 27001, NIS2, ANSSI…), format ouvert et personnalisable
- **Workflows** — circuit de validation et de suivi des actions
- **API-first** — pilotage par interface et par automation
- **Imports/exports** — échanges multi-formats pour s'intégrer à l'existant

## Le parti-pris UX

Un frontend réécrit de zéro (Next.js / React), dark, minimaliste :

- navigation claire par modules
- tableaux et formulaires dense mais lisibles
- cohérence visuelle via un design system strict
- prise en main rapide pour des profils non techniques (auditeurs, managers)

## Architecture (schéma)

```mermaid
flowchart TB
    subgraph FRONT["Frontend (PRISM)"]
        APP["Next.js / React"]
        UI["Design system dark"]
    end
    subgraph API["API"]
        R["REST API (API-first)"]
    end
    subgraph DATA["Données"]
        DB[("Base") ]
        Q[("Vecteurs / recherche")]
    end
    APP --> R
    R --> DB
    R --> Q
    UI --> APP
```

## Points clés

- **Open format** — frameworks et objets réutilisables, import/export
- **Réutilisabilité** — la conformité découplée des contrôles, réutilisable sur plusieurs référentiels
- **Automation** — pilotage par API pour connecter la GRC au reste de la chaîne

## À propos

Conçu par **Hamza DJOUDI** — Ingénieur Cybersécurité (GRC, ISO 27001, automatisation).

*Ce dépôt est une vitrine produit : présentation et architecture. Le code de la plateforme reste privé.*
