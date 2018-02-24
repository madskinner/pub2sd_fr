============
Contribuant
============

Les contributions sont les bienvenues, et elles sont grandement appréciées! Chaque
peu aide, et le crédit sera toujours donné.

Vous pouvez contribuer de plusieurs façons:

Types de contributions
----------------------

Signaler les bugs informatiques
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

signaler les bugs informatiques à https://github.com/madskinner/pub2sd2/issues.

Si vous signalez un bug, veuillez inclure:

* Tous les détails concernant votre configuration locale qui pourraient être utiles pour le dépannage.
* Étapes détaillées pour reproduire le bug.

Corriger les bugs
~~~~~~~~~~~~~~~~

Regardez les problèmes de GitHub pour les bugs. Tout ce qui est étiqueté "bug"
est ouvert à quiconque veut l'implémenter.

Implémenter les fonctionnalités
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Regardez à travers les problèmes de GitHub pour les fonctionnalités. Quoi que ce soit tagué avec "feature"
est ouvert à quiconque veut l'implémenter.

Écrire quelque documentation
~~~~~~~~~~~~~~~~~~~

Pub2SDwizard pourrait toujours utiliser plus de documentation, que ce soit
dans les documents officiels de Pub2SDwizard, dans docstrings,
ou même sur le Web dans les articles de blog, articles, et autres.

Soumettre des commentaires
~~~~~~~~~~~~~~~~~~~~~~~~~~~

La meilleure façon d'envoyer des commentaires est de déposer un problème à : 
https://github.com/madskinner/pub2sd2/issues.

Si vous proposez une fonctionnalité:

* Expliquer en détail comment cela fonctionnerait.
* Gardez la portée aussi étroite que possible, pour le rendre plus facile à mettre en œuvre.
* Rappelez-vous qu'il s'agit d'un projet dirigé par des bénévoles, et que les contributions
   sont les bienvenus :)

Commencer!
------------

Prêt à contribuer? Voici comment configurer `pub2sdwizard` pour le développement local.

1. Placez le repo `pub2sd2` sur GitHub.
2. Cloner votre fourche localement ::

    $ git clone git@github.com:votre_nom/pub2sd2.git

3. Installez votre copie locale dans un virtualenv. En supposant 
que virtualenvwrapper est installé, voici comment configurer votre fork pour le développement local::

    $ mkvirtualenv pub2sd
    $ cd pub2sd/
    $ python setup.py develop

4. Créer une branche pour le développement local::
    $ git checkout -b nom-de-votre-amélioration

   Vous pouvez maintenant effectuer vos modifications localement.

5. Lorsque vous avez fini de faire des changements, vérifiez que vos 
changements passent flake8 et les tests, y compris le test d'autres versions de Python avec tox::

    $ python setup.py test
    $ tox

   Pour avoir de la tox, il suffit de l'installer dans votre virtualenv.

6. Validez vos changements et déplacez votre branche vers GitHub::

    $ git add .
    $ git commit -m "Votre description détaillée de vos modifications."
    $ git push origin nom-de-votre-amélioration

7. Soumettez une "pull request" sur le site Web de GitHub.

Directives "Pull Request"
-----------------------

Avant de soumettre une "pull request", vérifiez qu'elle respecte les consignes suivantes:

1. La "pull request" devrait inclure des tests.
2. Si la 'pull request' ajoute une fonctionnalité, les documents doivent être mis à jour. Mettre
    votre nouvelle fonctionnalité dans une fonction avec une docstring, et ajoutez le
    fonctionnalité à la liste dans README.rst.
3. La 'pull request' devrait fonctionner pour Python 3.4, 3.5 et 3.6. Vérifier
    https://github.com/madskinner/pub2sd2/pull_requests
    et assurez-vous que les tests réussissent pour toutes les versions Python prises en charge.

