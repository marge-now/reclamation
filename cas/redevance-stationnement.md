# Cas 4 : quatre redevances de stationnement vieilles de trois ans, dans sa propre rue

Dossier réel, mené à Bruxelles en septembre 2026 avec Claude (Cowork et le navigateur). Anonymisé : la commune n'est pas nommée, ni l'organisme qui perçoit la redevance. Le cas est écrit par un second contributeur, pas par l'auteur des trois premiers : c'est le premier dossier apporté au repo de l'extérieur. En cours : contestations envoyées, réponses attendues.

## Le problème

Quatre avis de redevance de stationnement, reçus d'un coup, pour des stationnements datant de 2023. Tous dans la même rue. Celle où l'utilisateur habite, avec une carte de résident. Il n'y avait pas lieu de percevoir quoi que ce soit.

Le montant de chaque avis est petit. Le vrai problème est ailleurs : ne rien faire, c'est laisser quatre redevances se faire majorer, puis valider, puis arriver sous forme d'huissier à la porte quelques mois plus tard. Et contester, c'est retrouver le bon site, le bon formulaire, la référence de chaque avis, la carte, et tout retaper quatre fois. C'est exactement le litige qu'on repousse, puis qu'on paie pour avoir la paix.

## L'assessment (une ligne)

Le droit existe, la preuve tient en une pièce, le recours est en ligne et gratuit, le seul risque est le délai. Verdict : on y va, curseur doux, une contestation par avis, le jour même.

## Ce qui s'est passé

Les quatre avis sont photographiés. L'agent lit chaque photo : numéro d'avis, plaque, date, heure, rue, organisme émetteur, délai de contestation. Il vérifie dans le dossier que la carte de résident couvre la plaque, le secteur et les quatre dates de 2023. Il rédige une contestation de trois phrases par avis (le fait, le droit, la demande d'annulation), ouvre le formulaire de l'organisme dans le navigateur, remplit les champs, joint la carte, et s'arrête avant l'envoi.

Ce qui reste à l'utilisateur, pour chacun des quatre avis : relire, cocher le captcha, cliquer. Une photo, un clic. Le journal note la référence et la date d'envoi de chaque contestation.

Réponses de l'organisme : attendues au moment de la publication. Le cas sera complété.

## Ce qui a marché

- Photographier les avis au lieu de les recopier. L'agent lit mieux qu'on ne retape.
- Une seule pièce, réutilisée quatre fois : la carte de résident.
- Le formulaire piloté dans le navigateur jusqu'au captcha. Le coût d'une contestation tombe à une minute, ce qui change la décision : on conteste tout, y compris le petit avis qu'on aurait payé pour ne plus y penser.
- Traiter les quatre le même jour. Un avis contesté hors délai est un avis dû.

## Ce qui reste ouvert

- Pourquoi quatre avis de 2023 arrivent en 2026 : rappel de recouvrement tardif, ou avis jamais reçus à l'époque. La date de réception fait courir le délai, pas la date du stationnement ; à établir sur chaque avis.
- La cause des avis (carte enregistrée sur une mauvaise plaque, rue en limite de secteur, contrôle par scan-car qui ne voit pas la carte) : à établir, parce que tant qu'elle n'est pas corrigée, les avis reviennent.

## Ce que ça a changé dans le skill

La référence `stationnement.md` (France et Bruxelles, le vrai statut d'un avis de stationnement, les délais courts, les motifs qui portent), le template `contestation-stationnement.md`, et une règle dans le SKILL.md : quand le litige est une redevance de stationnement avec un droit prouvable, on ne fait pas d'assessment d'une page, on conteste le jour même.
