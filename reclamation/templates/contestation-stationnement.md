# Contestation d'un forfait post-stationnement ou d'une redevance de stationnement

Usage : le texte à coller dans le champ « motif » du formulaire en ligne (RAPO en France, formulaire de contestation de parking.brussels ou de la commune à Bruxelles), ou le corps d'un recommandé si le formulaire n'existe pas. Un avis, une contestation. Registre doux à moyen : l'organisme n'est pas un adversaire, c'est une base de données qui s'est trompée. Trois paragraphes, pas plus. Voir [../references/stationnement.md](../references/stationnement.md).

```
Objet : Contestation de l'avis {{numéro de l'avis}} du {{date de l'avis}}, véhicule {{plaque}}

Bonjour,

Je conteste l'avis référencé ci-dessus, établi le {{date}} à {{heure}}, {{rue, commune}}.

À cette date et à cet endroit, mon véhicule bénéficiait d'un droit de stationnement en cours de validité : {{carte de résident n° X valable du … au … pour le secteur … / abonnement … / ticket n° … de … à … / session {{application}} de … à …}}. La pièce justificative est jointe.

Je vous demande l'annulation de cet avis{{ et, le cas échéant, le remboursement de la somme de … € réglée le … pour éviter la majoration}}.

Bien cordialement,
{{Prénom NOM}}
{{Adresse}}

Pièces jointes :
1. Avis de paiement {{numéro}}
2. Certificat d'immatriculation
3. {{Carte de résident / abonnement / ticket / capture de la session}}
```

Variante quand la carte existe mais est enregistrée sur une autre plaque ou un autre secteur : ajouter une phrase, « La carte était enregistrée sur la plaque {{ancienne plaque}} ; la mise à jour a été faite le {{date}} (preuve jointe). » Et faire la mise à jour avant d'envoyer, pas après.

Après envoi : dans `journal.md`, la date, l'organisme, le numéro de l'avis, le récépissé ou la capture de confirmation, et la date à laquelle le silence vaut rejet (un mois en France pour le RAPO).
