De : https://github.com/facebook/chef-cookbooks/edit/master/CONTRIBUTING.md

# Contribuer aux livres de cuisine chef de Facebook

## Testez Markdown

Voici quelques  ~~ ~~ tests Markdown aromatisés à GitHub de @southgate.

:puis: | :ok_hand: | :froncement de sourcils: |
---------|----------|----------|
Félicitations énormes  | Moins de félicitations | Pas de félicitations

- [ ] Tâche 1
- [ ] Tâche 2
- [ ] Tâche 3

## Notre processus de développement
Ce référentiel est synchronisé à partir d'un référentiel interne. Nous acceptons absolument tirer
demande et traitera la fusion de manière appropriée.

Nous utilisons Foodcritic pour les tests de justesse chef et Rubocop pour le style Ruby
linting. Nos ensembles de règles sont synchronisés à la fois à l'interne et à l'externe pour
qualité et style de code cohérents pour tous.

## Contrat de licence des contributeurs (« CLA »)
Afin d'accepter votre demande de traction, nous avons besoin que vous soumettiez un CLA. Vous avez seulement besoin
de le faire une fois pour travailler sur l'un des projets open source de Facebook.

Complétez votre CLA ici: <https://code.facebook.com/cla>

## Pré-requis
Tout d'abord, merci pour votre intérêt à contribuer, nous accueillons favorablement les demandes de traction!

Avant d'envoyer une demande de traction à ce repo, il est important de se rappeler que le
Les API axées sur les attributs sont ici un modèle très différent de celui des autres
Livres. Afin de construire ce modèle, il ya une façon spécifique livres de cuisine ont besoin
à écrire.

Nous vous recommandons fortement de vous assurer que vous lisez [README.md](README.md)le
[Philosphy.md](https://github.com/facebook/chef-utils/blob/master/Philosophy.md).
Nous vous recommandons également d'avoir configuré un environnement qui utilise notre commande runlist
(livres de cuisine de base d'abord, tout le reste après).

Enfin, assurez-vous de suivre l'approche en 3 phases :

 * `attributes/` les fichiers configurent une API et ne touchent jamais les attributs d'un autre livre de cuisine.
 * `recipes/` ressources de configuration de fichiers (comme des modèles ou des services) et
   API (lire : définir les attributs des autres livres de cuisine)
 * Les attributs ne sont jamais consommés `runtime`à (aka  `converge time`).
   Par exemple,  `templates`il y a `ruby_blocks` ,  `whyrun_safe_ruby_blocks`ou
   `providers`.

## Questions
Nous utilisons les problèmes GitHub pour suivre les bogues publics. S'il vous plaît assurez-vous que votre description est
claires et ont suffisamment d'instructions pour être en mesure de reproduire le problème.

Facebook a un pour [programme de primes](https://www.facebook.com/whitehat/)le coffre-fort
divulgation des bogues de sécurité. Dans ces cas, s'il vous plaît passer par le processus
sur cette page et ne déposent pas de question publique.

## Envoi d'une demande de traction

Vous avez un correctif ou une fonctionnalité ? génial! Lorsque vous envoyez la demande de traction, nous vous suggérons
inclure une certaine sortie d'une course de chef applicable.

S'il s'agit d'une nouvelle API (attribut), veuillez vous assurer qu'elle est
livre de cuisine README.

Nous conserverons toutes les contributions aux mêmes normes de qualité et de style que les
code existant.


### Nouveaux livres de cuisine

Nous aimerions garder ce repo concentré sur « core » livres de cuisine qui gèrent la base
Os. Si vous souhaitez contribuer à un tel livre de cuisine, nous vous recommandons de commencer par
déposer un numéro d'abord pour éviter de dupliquer l'effort (nous pouvons en avoir un que nous pouvons
essayer d'open-source, ou d'autres personnes peuvent écrire un) avant de travailler sur elle.

Si vous souhaitez contribuer à un livre de cuisine qui ne fait pas partie de cette catégorie (p. ex.
gestion des choses de bureau ou d'autres services), alors nous vous suggérons de nous pointer vers un PR
sur un repo où vous souhaitez le garder et nous serons heureux de l'examiner et d'ajouter un
pointeur de votre repo dans notre 
[UNIVERSE.md](https://github.com/facebook/chef-cookbooks/blob/master/UNIVERSE.md)
fichier.

Nous utilisons le `fb_`préfixe pour désigner les livres de cuisine qui correspondent
ce modèle et proviennent de ce repo, mais n'hésitez pas à publier des livres de cuisine ailleurs
qui laissent rage ce modèle et utilisent d'autres préfixes.

## licence
En contribuant à ce référentiel, vous convenez que vos contributions seront
sous sa licence Apache 2.0.
