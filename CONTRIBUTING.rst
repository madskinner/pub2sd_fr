============
Contribuant
============

Les contributions sont les bienvenues, et elles sont grandement appr�ci�es! Chaque
peu aide, et le cr�dit sera toujours donn�.

Vous pouvez contribuer de plusieurs fa�ons:

Types de contributions
----------------------

Signaler les bugs informatiques
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

signaler les bugs informatiques � https://github.com/madskinner/pub2sd/issues.

Si vous signalez un bug, veuillez inclure:

* Tous les d�tails concernant votre configuration locale qui pourraient �tre utiles pour le d�pannage.
* �tapes d�taill�es pour reproduire le bug.

Corriger les bugs
~~~~~~~~~~~~~~~~

Regardez les probl�mes de GitHub pour les bugs. Tout ce qui est �tiquet� "bug"
est ouvert � quiconque veut l'impl�menter.

Impl�menter les fonctionnalit�s
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Regardez � travers les probl�mes de GitHub pour les fonctionnalit�s. Quoi que ce soit tagu� avec "feature"
est ouvert � quiconque veut l'impl�menter.

�crire quelque documentation
~~~~~~~~~~~~~~~~~~~

Pub2SDwizard pourrait toujours utiliser plus de documentation, que ce soit
dans les documents officiels de Pub2SDwizard, dans docstrings,
ou m�me sur le Web dans les articles de blog, articles, et autres.

Soumettre des commentaires
~~~~~~~~~~~~~~~~~~~~~~~~~~~

La meilleure fa�on d'envoyer des commentaires est de d�poser un probl�me � https://github.com/madskinner/pub2sd/issues.

Si vous proposez une fonctionnalit�:

* Expliquer en d�tail comment cela fonctionnerait.
* Gardez la port�e aussi �troite que possible, pour le rendre plus facile � mettre en �uvre.
* Rappelez-vous qu'il s'agit d'un projet dirig� par des b�n�voles, et que les contributions
   sont les bienvenus :)

Commencer!
------------

Pr�t � contribuer? Voici comment configurer `pub2sdwizard` pour le d�veloppement local.

1. Placez le repo `pub2sd2` sur GitHub.
2. Cloner votre fourche localement ::

    $ git clone git@github.com:votre_nom/pub2sd2.git

3. Installez votre copie locale dans un virtualenv. En supposant 
que virtualenvwrapper est install�, voici comment configurer votre fork pour le d�veloppement local::

    $ mkvirtualenv pub2sd
    $ cd pub2sd/
    $ python setup.py develop

4. Cr�er une branche pour le d�veloppement local::
    $ git checkout -b nom-de-votre-am�lioration

   Vous pouvez maintenant effectuer vos modifications localement.

5. Lorsque vous avez fini de faire des changements, v�rifiez que vos 
changements passent flake8 et les tests, y compris le test d'autres versions de Python avec tox::

    $ python setup.py test
    $ tox

   Pour avoir de la tox, il suffit de l'installer dans votre virtualenv.

6. Validez vos changements et d�placez votre branche vers GitHub::

    $ git add .
    $ git commit -m "Votre description d�taill�e de vos modifications."
    $ git push origin nom-de-votre-am�lioration

7. Soumettez une "pull request" sur le site Web de GitHub.

Directives "Pull Request"
-----------------------

Avant de soumettre une "pull request", v�rifiez qu'elle respecte les consignes suivantes:

1. La "pull request" devrait inclure des tests.
2. Si la 'pull request' ajoute une fonctionnalit�, les documents doivent �tre mis � jour. Mettre
    votre nouvelle fonctionnalit� dans une fonction avec une docstring, et ajoutez le
    fonctionnalit� � la liste dans README.rst.
3. La 'pull request' devrait fonctionner pour Python 3.4, 3.5 et 3.6. V�rifier
    https://github.com/madskinner/pub2sd/pull_requests
    et assurez-vous que les tests r�ussissent pour toutes les versions Python prises en charge.

