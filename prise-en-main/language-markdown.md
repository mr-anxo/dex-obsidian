# Language Markdown

## Présentation de MarkDown

1. Introduction
2. Syntaxe de base
3. Titres
4. Formatage du texte
5. Listes
6. Liens
7. Images
8. Code
9. Tableaux
10. Citations
11. Lignes horizontales
12. Échappement de caractères
13. Markdown étendu
14. Bonnes pratiques
15. Outils et éditeurs



Markdown est un langage de balisage léger créé par John Gruber en 2004. Il permet de formater du texte de manière simple et lisible, tout en étant facilement convertible en HTML. Markdown est largement utilisé pour la documentation, les README, les blogs, et les plateformes comme GitHub.

### Avantages de Markdown

* **Simplicité** : Syntaxe intuitive et facile à apprendre
* **Lisibilité** : Le texte source reste lisible même sans rendu
* **Portabilité** : Compatible avec de nombreux outils et plateformes
* **Rapidité** : Permet une écriture rapide sans quitter le clavier

## Syntaxe de base

### Titres

Markdown propose 6 niveaux de titres, similaires aux balises HTML h1-h6 :

```markdown
# Titre niveau 1
## Titre niveau 2
### Titre niveau 3
#### Titre niveau 4
##### Titre niveau 5
###### Titre niveau 6
```

**Syntaxe alternative pour les titres 1 et 2 :**

```markdown
Titre niveau 1
===============

Titre niveau 2
---------------
```

### Formatage du texte

#### **Emphase et importance**

```markdown
*Texte en italique* ou _Texte en italique_
**Texte en gras** ou __Texte en gras__
***Texte en gras et italique*** ou ___Texte en gras et italique___
~~Texte barré~~ (extension)
```

**Résultat :**

* _Texte en italique_
* **Texte en gras**
* _**Texte en gras et italique**_
* ~~Texte barré~~

#### Paragraphes et sauts de ligne

* **Paragraphe** : Séparez par une ligne vide
* **Saut de ligne** : Terminez une ligne par deux espaces ou utilisez `<br>`

```markdown
Premier paragraphe.

Deuxième paragraphe.

Ligne avec saut de ligne  
Nouvelle ligne.
```

### Listes

#### Listes non ordonnées

Utilisez `-`, `*`, ou `+` :

```markdown
- Élément 1
- Élément 2
  - Sous-élément 2.1
  - Sous-élément 2.2
- Élément 3
```

#### Listes ordonnées

Utilisez des nombres suivis d'un point :

```markdown
1. Premier élément
2. Deuxième élément
   1. Sous-élément 2.1
   2. Sous-élément 2.2
3. Troisième élément
```

#### Listes de tâches (extension)

```markdown
- [x] Tâche terminée
- [ ] Tâche en cours
- [ ] Tâche à faire
```

### Liens

#### Liens simples

```markdown
[Texte du lien](https://example.com)
[Texte du lien](https://example.com "Titre optionnel")
```

#### Liens de référence

```markdown
[Texte du lien][référence]
[Autre lien][1]

[référence]: https://example.com
[1]: https://example.com "Titre optionnel"
```

#### Liens automatiques

```markdown
<https://example.com>
<email@example.com>
```

#### Liens internes (ancres)

```markdown
[Aller à la section](#nom-de-la-section)
```

### Images

#### Syntaxe de base

```markdown
![Texte alternatif](chemin/vers/image.jpg)
![Texte alternatif](chemin/vers/image.jpg "Titre optionnel")
```

#### Images avec liens de référence

```markdown
![Texte alternatif][image-ref]

[image-ref]: chemin/vers/image.jpg "Titre optionnel"
```

#### Images cliquables

```markdown
[![Texte alternatif](chemin/vers/image.jpg)](https://example.com)
```

### Code

#### Code en ligne

Utilisez des backticks :

```markdown
Voici du `code en ligne` dans une phrase.
```

#### Blocs de code

Utilisez trois back ticks ou quatre espaces :

````markdown
```
Code sans coloration syntaxique
```

```javascript
// Code JavaScript avec coloration syntaxique
function hello() {
    console.log("Hello, World!");
}
```
````

#### Code indenté

```markdown
    Code indenté avec 4 espaces
    Deuxième ligne de code
```

### Tableaux

```markdown
| En-tête 1 | En-tête 2 | En-tête 3 |
|-----------|-----------|-----------|
| Cellule 1 | Cellule 2 | Cellule 3 |
| Cellule 4 | Cellule 5 | Cellule 6 |
```

#### Alignement des colonnes

```markdown
| Gauche | Centré | Droite |
|:-------|:------:|-------:|
| Texte  | Texte  | Texte  |
| Texte  | Texte  | Texte  |
```

### Citations

#### Citations simples

```markdown
> Ceci est une citation.
> Elle peut s'étendre sur plusieurs lignes.
```

#### Citations imbriquées

```markdown
> Citation principale
>> Citation imbriquée
>>> Citation doublement imbriquée
```

#### Citations avec formatage

```markdown
> **Citation importante**
> 
> Avec du *formatage* et du code : `example()`
```

### Lignes horizontales

Utilisez trois ou plus de ces caractères :

```markdown
---
***
___
```

### Échappement de caractères

Pour afficher littéralement des caractères spéciaux, utilisez l'antislash `\` :

```markdown
\*Texte avec astérisques littéraux\*
\[Crochets littéraux\]
\# Dièse littéral
```

#### Caractères à échapper

```
\ ` * _ { } [ ] ( ) # + - . ! |
```

### Markdown étendu

### Extensions communes

**Notes de bas de page**

```markdown
Texte avec note de bas de page[^1].

[^1]: Contenu de la note de bas de page.
```

#### **Définitions**

```markdown
Terme 1
: Définition du terme 1

Terme 2
: Définition du terme 2
```

#### **Mise en évidence de syntaxe**

```markdown
==Texte surligné== (certains moteurs)
```

**Indices et exposants**

```markdown
H~2~O (indice)
X^2^ (exposant)
```

### GitHub Flavored Markdown (GFM)

#### **Mentions et références**

```markdown
@utilisateur
#123 (référence à une issue)
```

#### **Émojis**

```markdown
:smile: :heart: :thumbsup:
```

### Bonnes pratiques

#### Structure et organisation

1. **Utilisez une hiérarchie logique** des titres
2. **Ajoutez une table des matières** pour les documents longs
3. **Utilisez des liens internes** pour la navigation
4. **Séparez les sections** avec des lignes horizontales si nécessaire

#### Formatage cohérent

1. **Choisissez un style** pour l'emphase (`*` ou `_`) et restez cohérent
2. **Utilisez des espaces** autour des éléments de liste
3. **Indentez correctement** les sous-éléments
4. **Ajoutez des lignes vides** autour des blocs de code et tableaux

#### Accessibilité

1. **Utilisez des textes alternatifs** descriptifs pour les images
2. **Créez des liens explicites** plutôt que "cliquez ici"
3. **Structurez correctement** avec les niveaux de titres

#### Performance et maintenance

1. **Optimisez les images** en taille et format
2. **Utilisez des liens relatifs** quand possible
3. **Vérifiez régulièrement** les liens externes
4. **Documentez vos conventions** dans un guide de style

### Outils et éditeurs

#### Éditeurs spécialisés

* **Typora** : Éditeur WYSIWYG
* **Mark Text** : Éditeur temps réel
* **Zettlr** : Pour la recherche académique
* **Obsidian** : Pour la prise de notes liée

#### Éditeurs de code avec support Markdown

* **Visual Studio Code** (avec extensions)
* **Sublime Text**
* **Atom**
* **Vim/Neovim**

#### Outils en ligne

* **Dillinger** : Éditeur en ligne
* **StackEdit** : Éditeur avec synchronisation cloud
* **HackMD** : Collaboration en temps réel

#### Extensions de navigateur

* **Markdown Viewer** : Pour Chrome/Firefox
* **Markdown Preview Plus** : Pour Chrome

#### Convertisseurs

* **Pandoc** : Convertisseur universel
* **Marked** : Bibliothèque JavaScript
* **markdown-it** : Parser JavaScript moderne

#### Validation et linting

* **markdownlint** : Vérification de style
* **markdown-link-check** : Vérification des liens
* **Vale** : Vérification orthographique et stylistique

### Ressources complémentaires

#### Spécifications

* **CommonMark** : Spécification standardisée
* **GitHub Flavored Markdown** : Extension de GitHub
* **MultiMarkdown** : Extension avec fonctionnalités avancées

#### Cheat Sheets

* Cartes de référence rapide disponibles en ligne
* Aide-mémoires imprimables
* Extensions de navigateur avec syntaxe

#### Communautés

* Forums spécialisés
* Groupes d'utilisateurs
* Canaux Discord/Slack dédiés

***

_Cette documentation couvre les aspects essentiels de Markdown. Pour des cas d'usage spécifiques, consultez la documentation de votre plateforme ou outil particulier._
