# PyForm

## Description
PyForm est un outil de génération automatique de formulaires pour les projets Django. Il facilite la création de formulaires basés sur des modèles de classe Django, en prenant en compte le type des champs et les relations.

## Installation
Pour installer PyForm, exécutez simplement la commande suivante :

```
pip install pyform
```

## Utilisation
Après l'installation, vous pouvez utiliser PyForm directement depuis la ligne de commande de Django. Voici quelques exemples de commandes :

### Générer un Formulaire pour la Partie Publique
Pour générer un formulaire basé sur un modèle Django pour la partie publique :

```
python manage.py createform ModelName --app AppName
```

Remplacez `ModelName` par le nom de votre modèle Django et `AppName` par le nom de l'application contenant le modèle.

### Générer un Formulaire pour l'Administration
Pour générer un formulaire destiné à être utilisé dans l'interface d'administration de Django :

```
python manage.py createform ModelName --app AppName --for-admin
```

Cette commande ajoutera le modèle à l'administration de Django.

### Options Avancées
- Pour générer un formulaire HTML au lieu d'un formulaire Django :

  ```
  python manage.py createform ModelName --app AppName --type html
  ```

- Pour spécifier une extension de fichier personnalisée pour le formulaire HTML :

  ```
  python manage.py createform ModelName --app AppName --type html --ext xml
  ```

---

## Fonctionnalités
- Génération automatique de formulaires Django ou HTML à partir de modèles.
- Mise à jour des fichiers `views.py` et `urls.py`.
- Prise en charge des formulaires pour la partie publique et l'administration.
- Vérification de l'existence de formulaires existants avec option de remplacement.
- Paramètres personnalisables pour la génération de formulaires.

## Contribution
Les contributions au projet sont les bienvenues. Veuillez consulter les guidelines de contribution avant de soumettre une pull request.

## Licence
Ce projet est sous licence MIT. Voir le fichier LICENCE pour plus de détails.