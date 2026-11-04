![1793786542861](image/Tp3/1793786542861.png)

![1793787379400](image/Tp3/1793787379400.png)

**Question :** Que gagne-t-on à décrire le lancement dans un fichier plutôt que dans une longue commande ?

toute la configuration est centralisée et versionnée dans Git, évitant les erreurs de frappe et permettant de tout démarrer avec une seule commande.


![1793795911060](image/Tp3/1793795911060.png)


![1793795981856](image/Tp3/1793795981856.png)


**Questions :** Pourquoi `build` attend-il `test` ? Pourquoi éviter le tag `latest` en production ?

* **Pourquoi `build` attend-il `test` ?**

  Pour éviter de compiler et publier une image contenant des bugs si les tests échouent : on ne livre que du code vérifié et fonctionnel.

  * **Pourquoi éviter le tag `latest` en production ?**

  Parce qu'il n'est pas figé : son contenu change à chaque nouveau build, ce qui empêche de savoir exactement quelle version tourne et rend impossible tout retour arrière (rollback) fiable.

![1793796398453](image/Tp3/1793796398453.png)

![1793796678411](image/Tp3/1793796678411.png)


**Question :** Quel est l'avantage d'une image versionnée par rapport à « le code de ma machine » ?

Elle garantit que l'application tourne exactement de la même manière partout, sans dépendre de la configuration ou des fichiers locaux de votre machine.
