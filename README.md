<h1 align="center">Réclamation</h1>

<p align="center">
  <b>Un skill pour agents IA qui mène vos litiges du quotidien, en français, sans avocat.</b>
</p>

<p align="center">
  Parce que l'assureur, l'agence et le loueur comptent sur votre fatigue. Le skill, lui, ne se fatigue pas.
</p>

<p align="center">
  <a href="https://github.com/marge-now/reclamation/stargazers"><img src="https://img.shields.io/github/stars/marge-now/reclamation?style=flat&color=F2B41A" alt="GitHub stars"></a>
  <img src="https://img.shields.io/badge/cas%20r%C3%A9els-4-blue" alt="4 cas réels">
  <img src="https://img.shields.io/badge/evals-6%20cas%20de%20test-lightgrey" alt="6 cas de test">
  <a href="https://github.com/marge-now/reclamation/blob/main/LICENSE"><img src="https://img.shields.io/badge/licence-MIT-blue" alt="MIT"></a>
  <img src="https://img.shields.io/badge/langue-fran%C3%A7ais-lightgrey" alt="français">
  <a href="https://marge.now"><img src="https://img.shields.io/badge/un%20projet-Marge-F2B41A" alt="Marge"></a>
</p>

---

## Qu'est-ce que c'est ?

Réclamation est un skill pour agents IA ([Claude Code](https://claude.com/product/claude-code), [Claude Cowork](https://claude.com/product/cowork), [Codex](https://openai.com/codex/), [Cursor](https://cursor.com), et tout agent capable de lire un dossier de fichiers Markdown) qui prend en charge un litige de particulier ou de petite entreprise : une assurance qui refuse de rembourser, un bailleur qui laisse traîner un danger, un prestataire qui ne livre pas et prélève quand même, une redevance de stationnement reçue alors que vous aviez le droit de vous garer.

Il fait ce qu'un ami juriste et organisé ferait pour vous, dans l'ordre :

1. **L'assessment** : quel est vraiment le problème, ce que ça coûte, ce qu'on peut récupérer, ce que ça demande, et si ça vaut le coup d'y aller. Vous décidez.
2. **Le dossier** : un brain du litige (parties, chronologie, pièces, deadlines) et un journal des envois avec preuves, tenus à jour à chaque épisode.
3. **Les courriers** : réclamation, mise en demeure, relance d'escalade, saisine du médiateur, signalement à la mairie, résolution de contrat, contestation de stationnement. Rédigés dans un registre précis, vérifiés juridiquement, relus pour ne pas sentir l'IA.
4. **L'action** : le recommandé déposé sur laposte.fr sans imprimante, le dossier monté sur le site du médiateur, le formulaire de contestation rempli jusqu'au captcha, les drafts prêts dans votre boîte mail. Vous payez, vous uploadez, vous envoyez. Jamais lui.
5. **L'escalade** : un cran à la fois, annoncé dans le courrier précédent, exécuté à la date dite.

---

## Les dossiers réels

Le skill est né de vrais litiges, menés avec Claude à l'été 2026, à côté du lancement d'une boîte et sans aucun goût pour la paperasse. Chacun est raconté dans [`cas/`](cas/), du premier mail à l'issue, avec ce qui a marché, ce qui a foiré, et ce que ça a changé dans le skill.

| Cas | Le litige | L'issue |
|---|---|---|
| [L'assurance du chien](cas/assurance-chien.md) | Un assureur animalier pose une exclusion à vie sur l'estomac d'un chiot de 8 mois, pour une diarrhée antérieure au contrat | Saisine du médiateur recevable, mémoire de 19 pièces déposé, position attendue au printemps 2027 |
| [Le vélo en location longue durée](cas/velo-lld.md) | Quatre pannes, un loueur qui renvoie vers son fournisseur et prélève quand même | Contrat résolu, 494,90 € remboursés sur 494,90 €, en 26 jours, zéro avocat |
| [Le balcon condamné](cas/balcon.md) | Une agence interdit l'accès à un balcon de 27 m² « jusqu'à nouvel ordre » et envoie des menuisiers réparer du verre | Rapport de bureau de contrôle obtenu, mairie dans le dossier, propriétaire rallié |
| [Les redevances de stationnement](cas/redevance-stationnement.md) | Quatre avis de redevance datant de 2023, reçus d'un coup, pour une voiture garée dans sa propre rue, carte de résident en poche | Quatre contestations préparées par l'agent depuis une photo, envoyées le jour même, réponses attendues |

Coût total des trois premiers dossiers : cinq recommandés à 8,60 €, zéro avocat.

---

## Installation

Copiez-collez dans votre agent :

```
Installe le skill du repo github https://github.com/marge-now/reclamation
puis lance un assessment sur mon litige
```

L'agent clone le repo, installe le skill, et vous demande le contrat, les échanges et la chronologie pour faire l'assessment.

Le skill est du Markdown. Pas de dépendance, pas de script, pas de clé API. Il marche partout où un agent peut lire des fichiers. Le dépôt du recommandé, le formulaire du médiateur et la contestation de stationnement demandent un agent capable de piloter un navigateur (Claude in Chrome, ou le navigateur intégré de Cowork).

### À la main, par plateforme

Copiez le dossier `reclamation/` dans le dossier de skills de votre agent, et créez un dossier `dossiers/` dans le dossier de travail de votre conversation (le projet Cowork, ou le répertoire où vous lancez l'agent). C'est là que vivent vos litiges, un sous-dossier par litige, et ils ne sont jamais commités.

| Plateforme | Où copier `reclamation/` |
|---|---|
| **Claude Code** | `~/.claude/skills/` |
| **Claude Cowork / claude.ai** | Réglages → Capabilities → Skills, uploader un `.zip` du dossier `reclamation/` (le `SKILL.md` doit être à la racine du zip) |
| **Codex** | `~/.codex/skills/` |
| **Cursor** | `~/.cursor/skills/` |
| **Windsurf** | `~/.windsurf/skills/` |
| **Cline** | `~/.cline/skills/` |
| **Mistral Vibe** | `~/.vibe/skills/` |

Le skill est autonome : pas de ressource partagée, pas de lien symbolique. Un zip du dossier suffit.

---

## Exemples

```
> Mon assureur a posé une exclusion sur mon chien pour un épisode de diarrhée antérieur à la souscription. Est-ce que ça vaut le coup de contester ?

> Voilà le contrat de location de mon vélo et les emails du loueur. Le vélo est en panne depuis 3 semaines, ils continuent à prélever. Fais-moi l'assessment.

> Mon agence m'interdit l'accès à mon balcon depuis 2 mois « en attendant l'assurance ». Rédige la mise en demeure.

> Voilà les photos de trois avis de redevance de stationnement et ma carte de résident. Conteste-les.

> Le médiateur n'a pas répondu depuis 6 semaines. Qu'est-ce qu'on fait ?

> Ils ont répondu, voilà leur mail. Cran suivant ou on accepte ?

> Prépare le recommandé sur laposte.fr, je paierai moi-même.
```

---

## Ce que le skill sait faire, et ce qu'il refuse

**Il sait** : lire vos contrats et conditions générales en entier, connecter un courrier de l'adversaire à l'article qui le contredit, tenir la chronologie et les deadlines, écrire dans le registre qui fait bouger un service réclamations, et préparer chaque action jusqu'au dernier clic avant paiement ou envoi.

**Il refuse** : de citer un article de loi qu'il n'a pas vérifié à la source, d'envoyer un courrier ou un email à votre place, de payer, de menacer de publier quelque chose sous condition de paiement (c'est la ligne du chantage), et de vous pousser dans un combat dont l'assessment dit qu'il ne vaut pas le coup.

Le curseur d'agressivité a trois positions, **doux**, **moyen**, **épicé**. Vous choisissez le départ, le skill ajuste d'après les faits : deadlines ignorées, aveux écrits, temps écoulé. Trop agressif, on est ridicule. Trop soumis, on se fait marcher dessus.

---

## Structure

```
reclamation/
  SKILL.md            le routeur : prérequis, échéances, domaine → référence, structure de réponse
  references/         la méthode, le registre, le droit par domaine (assurance, logement, B2B,
                      stationnement), les process (laposte.fr, médiateur)
  templates/          brain de dossier, journal, et les courriers
  evals/              cas de test au format anthropics/skills
cas/                  les litiges réels, anonymisés, du premier mail à l'issue
dossiers/             vos litiges (jamais commités)
```

---

## Avertissement

Ce skill a été écrit par des non-juristes, pour des non-juristes, à partir de dossiers réels. Il aide à comprendre un litige, à l'organiser et à écrire juste. Il ne remplace pas un avocat, il vous dit quand il en faut un : montant important, procédure engagée contre vous, adversaire représenté, ou tout ce qui touche au pénal.

Chaque article cité est vérifié sur Légifrance au moment de l'écriture du courrier. Le droit français bouge, le skill le sait, et il le signale quand il n'est pas sûr.

---

## Un projet Marge

[Marge](https://marge.now) est un cabinet de conseil en IA agentique pour les entreprises françaises et belges de 50 à 1 000 salariés. Réclamation est notre premier projet open source : la méthode qu'on applique en entreprise (un brain, un journal, des skills qui lisent, écrivent et agissent), appliquée à la paperasse qui pourrit la vie de tout le monde. Un litige, c'est la plus petite mission agentique possible.

La suite des dossiers se raconte chaque jeudi dans [la newsletter Marge](https://marge.beehiiv.com/subscribe), avec un atelier par semaine. L'atelier Réclamation, avec les prompts, est sur [marge.now/ateliers/reclamation](https://marge.now/ateliers/reclamation/).

Inspiré par [paperasse](https://github.com/romainsimon/paperasse), qui a montré que des skills en Markdown pouvaient faire le travail d'un cabinet.

---

## Contribuer

La meilleure contribution est un litige que vous avez mené avec le skill, anonymisé, raconté du premier mail à l'issue. Voir [CONTRIBUTING.md](CONTRIBUTING.md). Licence MIT.

### Forks par pays

Le skill est écrit pour le droit français, avec une première ouverture belge (la redevance de stationnement à Bruxelles). Un `reclamation-be` complet (Ombudsman des assurances, justice de paix, bail bruxellois) est le premier fork qu'on attend. Ouvrez une issue pour que le vôtre soit listé ici.

---

## Remerciements

- **Le service réclamations**, pour l'accusé de réception le jour même et la réponse quatre-vingt-onze jours plus tard.
- **Le service sinistres**, pour avoir répondu à la place du service réclamations, ce qui ne compte pas.
- **Les deux menuisiers**, venus constater que du verre n'est pas du bois.
- **La Poste**, pour le recommandé à 8,60 € sans imprimante. Sincèrement, celui-là.
- **Le médiateur**, pour avoir précisé que le numéro de demande n'est pas un numéro de dossier. On aurait aimé le savoir le 22 juin.

---

## Star History

<a href="https://www.star-history.com/#marge-now/reclamation&Date">
  <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=marge-now/reclamation&type=Date" width="100%">
</a>

---

<p align="center">
  <i>Un dossier tenu se gagne rarement au tribunal. Il se gagne le jour où l'adversaire comprend que vous ne lâcherez pas.</i>
  <br>
  Fait à Lille et à Bruxelles, entre deux recommandés | <a href="LICENSE">Licence MIT</a>
</p>
