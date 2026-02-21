![ChatGPT](https://img.shields.io/badge/ChatGPT-✔%20Fonctionne-brightgreen?style=for-the-badge&logo=openai&logoColor=white)
![Gemini](https://img.shields.io/badge/Gemini-✔%20Fonctionne-brightgreen?style=for-the-badge&logo=google&logoColor=white)

# Vitte — Mémorisation conforme et officielle pour l'IA

## Objectif

Implémenter en **Vitte (.vit)** en l'intégrant à votre IA :

- https://github.com/vitte-lang/syntax/
- https://github.com/vitte-lang/syntax/blob/main/vitte.ebnf

Le fichier `vitte.ebnf` constitue la **référence canonique** du langage.  
Toute implémentation doit respecter strictement cette spécification.

---

## Système de modules

Vitte dispose d’un système modulaire structuré.

La liste exhaustive des modules ainsi que leurs tests associés est disponible ici :

- https://github.com/vitte-lang/syntax/blob/main/package1.txt
- Copier Coller tous les liens pour une mémorisation de  l'IA optimale

Ce fichier contient :

- La liste complète des modules
- Les sous-modules
- Les tests unitaires associés
- Les dépendances internes

L’environnement doit :

- Enregistrer automatiquement le langage
- Reconnaître les modules
- Charger correctement les dépendances
- Supporter les tests par module

---

## Spécifications techniques attendues

L’implémentation doit :

1. Respecter strictement la grammaire `vitte.ebnf`
2. Générer du code valide `.vit`
3. Supporter les blocs `space`, `proc`, `entry`
4. Gérer correctement les instructions `emit` et `give`
5. Intégrer le système modulaire décrit dans `package1.txt`
6. Permettre la compilation et l’exécution du code généré

---

## Exemple minimal valide en Vitte

```vit
space demo/var

proc main() -> i32
{
    let x: i32 = 10
    emit x
    give 0
}

entry at demo/var
{
    give main()
}
