# Contribuer

Le repo vit de dossiers réels. La meilleure contribution, c'est un litige que vous avez mené avec le skill, anonymisé, raconté du premier mail à l'issue, dans `cas/`. Ce qui a marché, ce qui a foiré, et ce que le skill aurait dû savoir.

## Ce qui est bienvenu

- Un nouveau cas dans `cas/` (voir le format des trois existants : contexte, chronologie, ce qui a marché, ce qui a foiré, ce que ça a changé dans le skill).
- Un nouveau domaine dans `references/` (téléphonie, énergie, voyage, banque, artisan qui ne finit pas le chantier). Un fichier, même structure que `assurance.md` : le parcours amiable obligatoire, le médiateur compétent, les 3 ou 4 articles qui portent, les pièges de délai.
- Un template de courrier manquant.
- Une correction juridique, avec la source Légifrance ou la jurisprudence en lien.
- Un cas de test dans `evals/evals.json`.

## Ce qui ne passe pas

- Un article de loi sans lien vers sa source.
- Un cas avec des noms de personnes physiques (salariés de l'adversaire, propriétaires, voisins). Les raisons sociales sont retirées aussi par défaut.
- Un template qui menace, insulte, ou conditionne un paiement à un silence public.
- Un domaine qui relève du pénal, du droit de la famille ou du droit du travail : ce n'est pas le périmètre, et ça demande un avocat.

## Style

Le skill s'adresse à quelqu'un qui a peur de son dossier. Chaque référence doit pouvoir être lue par quelqu'un qui n'a jamais ouvert un code. Phrases courtes, un article par point, entre parenthèses en fin de phrase. Pas de tiret long. Pas d'italique. Pas de formules d'IA (« il ne s'agit pas de X mais de Y », les triplets de synonymes, « sans plus attendre »).

## Un fork pour votre pays

Le skill est écrit pour le droit français, avec une première ouverture belge (la redevance de stationnement à Bruxelles). Si vous l'adaptez à un autre droit (belge, suisse, québécois), faites un fork nommé `reclamation-<pays>` et ouvrez une issue ici pour qu'il soit listé dans le README. La méthode (assessment, brain, journal, escalade, registre) ne change pas d'un pays à l'autre ; les références et les médiateurs, si.

## Process

Fork, branche, pull request. Décrivez le dossier qui a motivé la contribution, même en deux lignes.
