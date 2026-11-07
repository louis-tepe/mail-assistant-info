# Mail Assistant

Pages publiques ([présentation](https://louis-tepe.github.io/mail-assistant-info/), [confidentialité](https://louis-tepe.github.io/mail-assistant-info/privacy.html), [conditions](https://louis-tepe.github.io/mail-assistant-info/terms.html)) d’un outil personnel que j’ai conçu pour trier ma boîte Gmail. Le code de l’outil reste privé.

## Ce que fait l’outil

- Il classe chaque message Gmail dans une famille et signale ceux qui sont à traiter ou à vérifier.
- Il n’agit que par libellés et par archivage réversible, sous des règles que j’approuve une à une.
- Il n’envoie aucune réponse, ne supprime aucun message et ne marque rien comme lu ; Gmail reste l’interface.

## Repères mesurés

- Mise en service le 15 octobre 2026 : toute la boîte reprise ; 0,3 % des messages laissés incertains, pour vérification humaine.
- Accord de catégorie de 95,5 % sur 488 messages de référence contrôlés à l’aveugle, et de 88 % sur 100 cas rares (qualification d’octobre 2026 ; le modèle actuel, Liquid d1-ultra, a été requalifié sur le même corpus).
- Archivage testé en réel puis restauré : cinq messages, libellés rétablis à l’identique, aucun conflit.

Méthode : 500 messages de la boîte ont reçu une catégorie de référence attribuée à la main avant toute prédiction du modèle ; douze associations erronées ont été exclues, d’où 488 références. Les 100 cas rares, sans recouvrement avec les premiers, ont été lus de la même façon, sans prédiction montrée. Limites : les pièces jointes ne sont pas lues, et une référence humaine peut elle-même être fausse.

## Stack

TypeScript, API Gmail (OAuth), modèle de langage Liquid d1-ultra via OpenRouter, service local planifié, sauvegarde chiffrée.
