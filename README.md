# Mail Assistant

Pages publiques ([présentation](https://louis-tepe.github.io/mail-assistant-info/), [confidentialité](https://louis-tepe.github.io/mail-assistant-info/privacy.html), [conditions](https://louis-tepe.github.io/mail-assistant-info/terms.html)) d’un outil personnel que j’ai conçu pour trier ma boîte Gmail. Le code de l’outil reste privé.

## Ce que fait l’outil

- Il classe chaque message Gmail dans une famille et signale ceux qui sont à traiter ou à vérifier.
- Il n’agit que par libellés et par archivage réversible, sous des règles que j’approuve une à une.
- Il n’envoie aucune réponse, ne supprime aucun message et ne marque rien comme lu ; Gmail reste l’interface.

## Repères mesurés

- Mise en service le 15 octobre 2026 : 14 638 messages repris, dont 14 595 classés et 43 laissés incertains.
- Accord de catégorie de 95,5 % sur 488 messages de référence contrôlés à l’aveugle, et de 88 % sur 100 cas rares.
- Archivage testé en réel puis restauré : cinq messages, libellés rétablis à l’identique, aucun conflit.

## Stack

TypeScript, API Gmail (OAuth), modèle de langage via une passerelle d’IA, service local planifié, sauvegarde chiffrée.
