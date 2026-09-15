# Stationnement : contester un forfait post-stationnement (France) ou une redevance (Bruxelles)

Tiré d'un dossier réel : plusieurs avis reçus pour une voiture garée dans sa propre rue, alors qu'une carte de résident était en cours de validité (voir `cas/redevance-stationnement.md`). Le cas le plus fréquent : le droit de stationner existait, la base de données ne le savait pas.

Le mot « amende » est faux dans les deux pays, et ça change tout : un forfait post-stationnement en France et une redevance de stationnement à Bruxelles sont des redevances d'occupation du domaine public, pas des sanctions pénales. Pas de points, pas de casier, pas de tribunal de police. Un recours administratif, en ligne, avec des pièces. C'est le litige le plus rapide du skill : dix minutes de préparation, un formulaire, un captcha.

## Ce qui est hors périmètre

Une contravention au sens pénal (stationnement gênant ou dangereux, arrêt sur trottoir, place réservée aux personnes handicapées, en France sur avis de l'ANTAI ; en Belgique une amende SAC ou une perception immédiate de la police) suit un autre parcours : requête en exonération ou contestation devant le tribunal de police. Le skill le dit et s'arrête là. Voir le SKILL.md, section périmètre.

## France : le forfait post-stationnement (FPS)

### Ce que c'est

Depuis 2018, le stationnement payant sur voirie est une redevance fixée par chaque commune. Ne pas payer, ou payer insuffisamment, déclenche un forfait post-stationnement (art. L.2333-87 du Code général des collectivités territoriales). L'avis de paiement est envoyé par l'ANTAI ou par le prestataire de la commune. À Paris, le montant est celui de six heures de stationnement (75 € en zone 1, 50 € en zone 2, minoré de 30 % si payé sous 9 jours).

### Le recours, dans l'ordre

1. **Le RAPO, recours administratif préalable obligatoire.** Un mois à compter de la notification de l'avis (art. R.2333-120-13 du CGCT ; à Paris, la notification est comptée à la date de l'avis plus cinq jours). En ligne sur le site indiqué sur l'avis (à Paris : teleservices.paris.fr/rapo), ou par recommandé avec avis de réception à l'adresse RAPO de l'avis. Pièces : l'avis de paiement, le certificat d'immatriculation, et la preuve du droit de stationner (le ticket ou le reçu de l'application ; un relevé bancaire est refusé ; la carte de résident ou l'abonnement en cours de validité). L'administration a un mois pour répondre. Son silence vaut rejet.
2. **La CCSP, Commission du contentieux du stationnement payant** (tribunal du stationnement payant, à Limoges). Un mois après la décision de rejet du RAPO, ou après le silence d'un mois. En ligne ou par recommandé. Pas d'avocat obligatoire. Copies de l'avis et des échanges du RAPO.
3. **Pendant le recours, le délai de paiement continue de courir.** Le RAPO ne suspend rien : au-delà de trois mois, le FPS est majoré. Payer le FPS contesté évite la majoration ; il est remboursé si le recours aboutit. À dire à l'utilisateur dans l'assessment, il décide.

### Les motifs qui portent

- Un droit de stationner qui existait : carte ou abonnement de résident valide, ticket ou session mobile en cours, carte mobilité inclusion stationnement. La preuve datée fait tout.
- Le véhicule vendu, volé, ou la plaque usurpée avant les faits : certificat de cession et accusé ANTS, ou dépôt de plainte.
- Une erreur matérielle sur l'avis : plaque, lieu, heure.

### Les pièges

- **L'abonnement résident enregistré sur une mauvaise plaque ou une mauvaise zone.** L'avis arrive quand même. Le RAPO avec la preuve d'abonnement suffit, et il faut corriger l'abonnement dans la foulée, sinon le prochain avis arrive la semaine suivante.
- **Un avis par passage.** Plusieurs avis pour le même stationnement se contestent chacun séparément, un RAPO par avis, avec les mêmes pièces.
- **Le délai d'un mois court dès la notification**, pas dès le jour où on ouvre le courrier. Sur un avis reçu tard, on conteste d'abord, on discute ensuite.

## Bruxelles : la redevance de stationnement

### Ce que c'est

Chaque commune bruxelloise fixe une redevance forfaitaire pour un stationnement sans titre valable ; elle est perçue soit par l'agence régionale parking.brussels (Ixelles, Anderlecht, Evere, Ganshoren, Jette, Koekelberg, Schaerbeek, Berchem-Sainte-Agathe, Saint-Gilles, Molenbeek, Forest, Watermael-Boitsfort, Woluwe-Saint-Pierre), soit par la commune elle-même (Bruxelles-Ville, Etterbeek, Uccle, Auderghem, Saint-Josse, Woluwe-Saint-Lambert). L'avis (« retributie ») est laissé sur le pare-brise puis envoyé par courrier.

### Le recours

1. **La contestation en ligne**, sur le formulaire de l'organisme qui a émis l'avis : le formulaire de contestation de parking.brussels (identification par itsme, ou par compte avec copie de la carte d'identité et du certificat d'immatriculation), ou le formulaire de la commune (Bruxelles-Ville : brucity.cityenforcement.com, sous 10 jours calendrier à compter de la réception de l'avis). Référence de l'avis, plaque, et la pièce qui prouve le droit : carte de riverain valide, ticket, session d'application.
2. **Le paiement dans le délai suspend le recouvrement et n'empêche pas la contestation** (parking.brussels le dit expressément). Ne pas payer déclenche des frais administratifs par rappel, puis l'huissier. Sur un petit montant, payer puis contester est souvent le bon ordre.
3. **Sans réponse ou en cas de rejet**, la contestation se poursuit par courrier au service juridique de l'organisme. Une redevance est une créance civile : si l'organisme poursuit, c'est en principe devant le juge de paix, pas le tribunal de police. À vérifier sur l'avis et la réponse reçus.

### Les pièges

- **La carte de riverain est attachée à une plaque et à un secteur.** Un changement de voiture, une plaque temporaire, ou une rue en limite de secteur suffisent à générer des avis. Vérifier la plaque enregistrée avant de contester, et corriger la carte en même temps.
- **Le délai est court** (10 jours à Bruxelles-Ville). Préparer les pièces avant le premier avis, pas après le troisième.
- **Deux organismes, deux formulaires.** L'avis indique lequel. Une contestation envoyée à la commune pour un avis de parking.brussels n'est pas traitée.

## Le mouvement avec un agent qui pilote le navigateur

C'est le litige où l'agent fait presque tout : lire l'avis sur une photo (numéro, plaque, date, heure, lieu, organisme, délai), vérifier le droit de stationner dans les pièces du dossier (carte, abonnement, ticket), rédiger la contestation en trois phrases (le fait, le droit, la demande d'annulation, les pièces jointes), ouvrir le bon formulaire, le remplir, et s'arrêter avant l'envoi. L'utilisateur relit, coche le captcha, envoie. Puis l'agent note dans le journal la date, l'organisme, la référence, et la date à laquelle l'absence de réponse vaut rejet.

Plusieurs avis, même droit : une contestation par avis, mêmes pièces, à la chaîne.

## Sources

- Code général des collectivités territoriales, art. L.2333-87 et R.2333-120-13 (Légifrance).
- Ville de Paris, « Le forfait post-stationnement et le RAPO » : paris.fr/pages/forfait-post-stationnement-et-recours-administratif-prealable-obligatoire-5260
- Institut national de la consommation, « Comment contester un avis de paiement de FPS » : inc-conso.fr
- parking.brussels, FAQ redevance de stationnement et processus de recouvrement : parking.brussels
- Ville de Bruxelles, « Stationnement, contestation d'une redevance » : bruxelles.be/stationnement-contestation-redevance

Chaque montant et chaque délai ci-dessus est celui observé à la date de rédaction (septembre 2026). Les communes changent leurs tarifs et leurs formulaires : vérifier sur l'avis reçu avant d'écrire.
