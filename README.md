## Structure du fichier JSON

Le fichier JSON contient une liste de recettes sous la clé `recipes`. Chaque recette est un objet avec les informations suivantes :

- `id`: Identifiant unique de la recette
- `name`: Nom de la recette
- `image`: URL d'une image représentative de la recette
- `description`: Brève description du plat
- `difficulty`: Niveau de difficulté de la recette (par exemple, "Facile", "Moyen", "Difficile")
- `category`: Catégorie de plat (par exemple, "Plat principal", "Dessert", etc.)
- `ingredients`: Liste des ingrédients nécessaires, chaque ingrédient ayant :
  - `name`: Nom de l'ingrédient
  - `quantity`: Quantité de l'ingrédient
  - `estimatedPrice`: Estimation du coût de l'ingrédient en monnaie locale
- `prepTime`: Temps de préparation en minutes
- `cookingTime`: Temps de cuisson en minutes
- `steps`: Liste des étapes de préparation de la recette
- `servings`: Nombre de personnes pour cette recette
- `totalBudget`: Budget total estimé pour la recette
- `dietaryTags`: Tags indiquant des caractéristiques diététiques de la recette (par exemple, "high-protein", "vegetarian", etc.)
- `allergens`: Liste des allergènes présents dans la recette (le cas échéant)

### Exemple de recette dans le fichier JSON

```json
{
  "id": "1",
  "name": "Ravitoto sy Henakisoa",
  "image": "https://i.pinimg.com/originals/6d/a5/68/6da56890f58bc3dbc6347ad14fe71c1a.jpg",
  "description": "Un plat traditionnel malgache à base de feuilles de manioc pilées et de porc.",
  "difficulty": "Moyen",
  "category": "Plat principal",
  "ingredients": [
    {
      "name": "Manioc Leaves",
      "quantity": "500g",
      "estimatedPrice": 2000
    },
    {
      "name": "Pork",
      "quantity": "400g",
      "estimatedPrice": 12000
    }
  ],
  "prepTime": 30,
  "cookingTime": 60,
  "steps": [
    "Clean and pound the manioc leaves",
    "Cut pork into chunks",
    "Cook pork until tender",
    "Add manioc leaves and simmer"
  ],
  "servings": 4,
  "totalBudget": 14000,
  "dietaryTags": ["high-protein"],
  "allergens": []
}
