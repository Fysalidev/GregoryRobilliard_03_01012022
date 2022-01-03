le système 7-1 pour une codebase plus simple à gérer

le directory base/
contient les fichiers qui définissent les fondations de votre site,
par exemple la police de caractères et les normes que vous voulez appliquer sur tout votre site,
telles que le box-sizing ;

components/
Utilisé pour ranger les blocs BEM qui sont plus indépendants, comme les boutons.
Alors que les layouts peuvent utiliser d’autres composants pour générer leurs contenus,
les composants, eux, sont plus élémentaires.
Par exemple, un formulaire doit être considéré comme un layout :
la mise en page est une fonction vitale du bloc et il utilise d’autres blocs pour fonctionner,
comme des boutons. En revanche, le bouton lui-même est un composant car il n’a besoin d’aucun autre composant pour remplir sa fonction ;

layouts/
Dossier où vous mettez vos blocs BEM qui contiennent ce qui est réutilisable,
par exemple un header pour les mises en page de grande taille ou un footer ;

pages/
contient les blocs de code qui ne s’appliquent qu’à une seule page.
Vous utilisez des boutons dans tout votre site,
en revanche votre page d’accueil comporte une section Citation et une grille de projets qui ne sont employés nulle part ailleurs.
En d’autres termes, pages/ contient des règles spécifiques à une seule page qui ne seront pas réutilisées ailleurs ;

themes/
C’est ici que vous stockez le code thématique,
par exemple un style customisé pour Noël ou pour l’été.
On ne l’utilisera pas dans notre site ;

utils/
Rangez vos variables,
fonctions, mixins et les %placeholders pour les extensions (si vous en utilisez);

vendors/
Directory pour des feuilles de style externes comme Bootstrap ou jQuery UI.
En gros, il s’utilise pour tout CSS venant de l’extérieur.
Utiliser des frameworks comme Bootstrap permet d’accélérer le développement d’un site,
car ils contiennent des feuilles de style prédéfinies pour des choses comme les formulaires ou des boutons.