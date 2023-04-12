En travaillant à plusieurs sur un projet Git, il est important d'harmoniser le code, de sorte qu'il n'y ait pas trop de subjectivité dedans.

Pour cela, on se repose souvent sur des conventions de style établies pour la plupart des langages. 


Et plutôt que de le faire manuellement avant chaque commit, on peut également opter pour les hooks de pre-commit.


Un hook pre-commit, c'est un ensemble d'instructions ou de programmes exécutés en amont d'un commit et qui doivent être tous en succès avant de faire un pre-commit. Si par exemple, on se rend compte qu'un fichier ne respecte pas la convention de style, cela permet donc de ne pas effectuer de commit.

En général, on réalise plusieurs vérifications pour chaque pre-commit.


✅ Un refactoring pour modifier le code sans toucher aux fonctionnalités (espaces en trop, sauts de lignes, etc).

✅ Un linter qui va vérifier que le code respecte les conventions de style (par exemple PEP 8 sous Python).

✅ Une analyse syntaxique de code, notamment pour vérifier les potentielles erreurs de sécurité (Sonarqube ou PyBandit).

✅ Une mise à jour automatique des meilleures pratiques par rapport à la version du langage utilisé (PyUpgade).

✅ Un vérificateur de type statique pour les langages qui n'en disposent pas (PyRight dont j'ai parlé la semaine dernière).



Toutes ces bonnes pratiques visent à harmoniser le travail collaboratif et surtout, éviter au maximum les bugs futurs qui pourraient intervenir à cause d'un manque de lisibilité dans le code, ou de pratiques devenues obsolètes.
