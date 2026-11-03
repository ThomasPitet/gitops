![1793709782637](image/Tp2/1793709782637.png)

![1793709992305](image/Tp2/1793709992305.png)

**Questions :** Quelle différence entre un linter (flake8) et un formateur (black) ? Pourquoi séparer `lint` et `test` en deux jobs ?



* **Flake8 (linter) :**vérifie les erreurs de code et de style (ex : variables inutilisées).
* **Black (formateur) :**reformate automatiquement l'agencement du code (espaces, retours à la ligne).

**Pourquoi 2 jobs séparés ?**

 Pour les exécuter en parallèle et identifier immédiatement si le problème vient du style (`lint`) ou du fonctionnement (`test`).
