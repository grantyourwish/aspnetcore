# Kit de démarrage FranceConnect - Fournisseur d'identité (FI) 
## Compatible avec l'authentification à deux facteurs, via application d'authentification (TOTP), ou via clé de sécurité (FIDO2)

Ce projet exemple propose un canevas de site web en [ASP.NET Core](https://dotnet.microsoft.com/learn/aspnet/what-is-aspnet-core "ASP.NET Core"), faisant office de fournisseur d'identité OpenIDConnect à l'aide de [IdentityServer](https://dotnetfoundation.org/projects/identityserver), pour pour identifier les internautes qui le souhaitent depuis FranceConnect.

Vous pouvez trouver sur ce répertoire **[la documentation associée](/Documentation)**, ainsi que le **[le guide de démarrage rapide](/Source/README.md)** afin d'exécuter le canevas localement.

La version utilisée est .NET Core 6.0 (LTS)

La documentation est en chantier, et des travaux sont en cours afin que le fournisseur de démonstration soit testable depuis les environnements d'integration FranceConnect.

Vous pouvez néanmoins découvrir et tester le fonctionnement du canevas et de ses capacités d'authentification forte à l'adresse <https://aka.ms/FranceConnect-FI>

### Organisation du répertoire.
Les différents éléments de documentation sont disponibles sous le dossier [/Documentation](/Documentation).

Les différentes versions publiées du canevas sont rapidement accessibles à l'aide des *tags* définis, permettant de retrouver l'état du répértoire pour une version donnée. 
L'onglet "Releases" sur la droite est utilisable pour consulter aisément celles-ci.

Les branches identifient les différent travaux en cours : *main* correspondant à la branche stable, develop à la branche de travail, et toute autre branche represente un ajout individuel en cours de développement.

Ce [schéma](/Documentation/Ressources/Branches.jpg) illustre le flux de travail. Le mode de contribution est également indiqué sous [CONTRIBUTING.md](/CONTRIBUTING.md)

### FranceConnect 
La plateforme [FranceConnect](https://franceconnect.gouv.fr/) est un système d’identification visant à faciliter l’accès des usagers aux services numériques de l’administration en ligne, en évitant à tout un chacun de devoir créer un nouveau compte lors de l’accès à un nouveau service et donc à se remémorer différents mots de passe pour l’ensemble des services accédés.

Pour cela, le système FranceConnect permet à chaque usager de disposer d’un mécanisme d’identification reconnu par les téléservices de l’administration au travers du bouton FranceConnect. Lors de l’accès à un nouveau service, et au-delà de la possibilité toujours proposée de s’inscrire vis-à-vis d’une autorité administrative que ne connaîtrait pas encore l’usager, le bouton permet de sélectionner une identité compatible dont l’usager disposerait déjà (impôts, assurance maladie, identité numérique la poste, etc.) et de l’utiliser dans ce contexte.

FranceConnect est porté par la direction interministérielle du numérique, ou DINUM, qui accompagne les ministères dans leur transformation numérique, conseille le gouvernement et développe des services et ressources partagées comme ici ce système d’identification et d’authentification en ligne de l’État, ou encore le réseau interministériel de l’État, data.gouv.fr ou api.gouv.fr.

La documentation d'implémentation du service FranceConnect est disponible sur le [portail partenaires](https://partenaires.franceconnect.gouv.fr/fcp/fournisseur-identite) fourni par la DINUM.


### Tierces Parties

Le projet présent se base sur la souche Open Source IdentityServer4 et incorpore du code de [IdentityServer4.Templates](https://github.com/IdentityServer/IdentityServer4.Templates). Des informations supplémentaires sont présentes dans les en-têtes des différents fichiers source, ainsi que sous [NOTICE.md](NOTICE.md)
