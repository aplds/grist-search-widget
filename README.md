# Widget de recherche de colonne pour Grist

Un simple champ de recherche pour Grist qui permet de rechercher dans une colonne spécifique et de naviguer parmi les résultats à l'aide de raccourcis clavier et de filtres intelligents.

Code source original : https://github.com/RemindZ/grist-search-widget

---

## Fonctionnalités

Saisissez un terme de recherche, et le widget trouve toutes les lignes correspondantes dans la colonne choisie. Utilisez les boutons Précédent/Suivant ou les raccourcis clavier pour passer d'un résultat à l'autre. Le widget indique également votre position dans les résultats (par exemple, "3 sur 7").

---

## Caractéristiques

- **Correspondance partielle ou exacte** : Basculez entre la recherche de texte n'importe où dans les cellules ou uniquement les correspondances exactes.
- **Raccourcis clavier** : Naviguez entre les résultats sans utiliser la souris.
- **Recherche avec temporisation (debounce)** : Un délai intelligent de 300 ms évite les ralentissements pendant la saisie.
- **Bouton Effacer** : Réinitialisez la recherche en un clic.
- **Navigation automatique** : Sélectionne automatiquement la ligne correspondante dans votre tableau.
- **Compteur de correspondances** : Sachez toujours où vous en êtes dans les résultats.

---

## Raccourcis clavier

- `Entrée` : Passer au résultat suivant.
- `Maj + Entrée` : Revenir au résultat précédent.
- `Échap` : Effacer la recherche et réinitialiser.

---

## Mode d'emploi

1. Ajoutez ce widget en tant que **Widget personnalisé** dans Grist avec un accès en **"Lecture de tableau"** (aplds.github.io/grist-search-widget).
2. Associez la colonne **SearchColumn** à la colonne de texte que vous souhaitez rechercher.
3. Commencez à taper pour lancer la recherche (la recherche s'effectue automatiquement au fur et à mesure de la saisie).
4. Utilisez le bouton bascule pour passer entre la correspondance partielle et exacte.
5. Cliquez sur Précédent/Suivant ou utilisez les raccourcis clavier pour naviguer dans les résultats.

---

## Modes de correspondance

- **Correspondance partielle** (par défaut) : Trouve "chat" dans "catégorie", "éparpillé", etc.
- **Correspondance exacte** : Ne correspond qu'aux cellules strictement égales à votre terme de recherche (insensible à la casse).

---
Idéal pour trouver et naviguer rapidement parmi des entrées spécifiques dans de grands tableaux.
