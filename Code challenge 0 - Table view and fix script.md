1- Faire une table custom extendant de task
2- Faire une vue nommer "patate" ou l'on voit :  puis créer un objet de ce format ( les champ avec un * doivent être mandatory) :
|first Column|Second Column|
|--|--|
|number (changer le numbering automatique pour qu'il soit de format : patato001000. voir/lire la doc de number maintenance ) |opened by (automatique) |
| assigned to* | State |
| assignement group | *custom String field named :* patato* |

|one row ------------------------------------------------------------------------------>|
|--|
| Short Description |
| Description* |

* ne pas mettre les noms en gras dans la vue, ils sont simplement pour aider la compréhension de la vue

3- Entrer 5 records sur la table avec des descriptions 
4- Rouler un fix script nommé patatoScript allant chercher sur chaque record le sys_id du assigned_to et le copier dans la description, à la suite de la description déjà inscrite (elle ne doit pas être effacée)