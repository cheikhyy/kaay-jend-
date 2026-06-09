# Backlog S3 — Kaay Jënd
## Sprint de construction · Juin 2026 · Bolt.new + Dify + GitHub

---

### HMW Définitif
"Comment pourrions-nous transformer la fin de cursus d'un étudiant étranger à Dakar en un moment de transmission organisée — en connectant proactivement vendeurs sur le départ et nouveaux arrivants au sein d'une même communauté de confiance, de façon à ce que chaque meuble trouve preneur avant le jour du départ, au juste prix, avec suffisamment de transparence pour que l'acheteur décide sans se déplacer inutilement ?"

---

## User Stories MUST
*(À construire obligatoirement en S3)*

#### US-01 — Publication d'annonce rapide
**Story :** En tant qu'Amina (vendeuse), je veux publier une annonce avec 4 photos guidées, un prix et ma date de départ en moins de 3 minutes depuis mon Android, afin de mettre mes meubles en vente sans effort même quand je suis pressée.
**Priorité :** MUST
**Outil :** Bolt.new
**Effort :** Moyen
**Adresse :** Pain Reliever — Galerie photo guidée en 4 angles imposés · Contrainte MVP 1 et 3
**Critère d'acceptation :** Une annonce complète (4 photos, prix, date de départ) peut être publiée en moins de 3 minutes sur un Android en réseau 3G simulé, sans erreur bloquante.

---

#### US-02 — Consultation des annonces par quartier
**Story :** En tant qu'Awa (acheteuse), je veux voir les annonces de meubles disponibles près de mon quartier, filtrées par type de meuble, afin de trouver rapidement ce dont j'ai besoin sans me déplacer inutilement.
**Priorité :** MUST
**Outil :** Bolt.new
**Effort :** Moyen
**Adresse :** Gain Creator — Installation rapide et sereine · Pain Reliever — Concentration géographique sur 1 à 2 quartiers
**Critère d'acceptation :** L'acheteuse peut filtrer les annonces par quartier (Mermoz, Fann, Liberté) et par type de meuble (lit, bureau, chaise, étagère) et obtenir des résultats en moins de 5 secondes.

---

#### US-03 — Vérification étudiant par email universitaire
**Story :** En tant qu'Awa (acheteuse), je veux voir un badge "étudiant vérifié" sur les annonces et profils vendeurs, afin d'acheter à quelqu'un de la même communauté étudiante sans risque d'arnaque.
**Priorité :** MUST
**Outil :** Bolt.new + vérification email (domaine universitaire)
**Effort :** Faible
**Adresse :** Pain Reliever — Badge étudiant vérifié · Hypothèse C1 et I1
**Critère d'acceptation :** Un vendeur qui s'inscrit avec une adresse email universitaire reconnue (.ucad.edu.sn, .esp.sn, .ism.sn…) reçoit automatiquement le badge "étudiant vérifié" visible sur son profil et toutes ses annonces.

---

#### US-04 — Contact vendeur depuis une annonce
**Story :** En tant qu'Awa (acheteuse), je veux contacter le vendeur directement depuis une annonce via un lien WhatsApp ou un numéro masqué, afin d'organiser une visite ou poser une question sans quitter la plateforme.
**Priorité :** MUST
**Outil :** Bolt.new + lien WhatsApp natif
**Effort :** Faible
**Adresse :** Pain Reliever — Galerie photo guidée réduit les visites inutiles sans les supprimer · Contrainte MVP — pas de messagerie in-app complexe
**Critère d'acceptation :** Un bouton "Contacter le vendeur" sur chaque annonce ouvre WhatsApp avec un message pré-rempli contenant le titre de l'annonce, sans exposer le numéro complet du vendeur si l'option masquage est activée.

---

#### US-05 — Transmission datée (date de départ + fenêtre de vente)
**Story :** En tant qu'Amina (vendeuse), je veux indiquer ma date de départ lors de la publication de mon annonce, afin que mes annonces soient mises en avant automatiquement 3 semaines avant mon départ auprès des acheteurs de mon quartier.
**Priorité :** MUST
**Outil :** Bolt.new (logique de mise en avant) + Dify (déclenchement automatique)
**Effort :** Élevé
**Adresse :** Gain Creator — Sérénité du départ · Pain Reliever — Fenêtre de vente prioritaire · Hypothèse C3
**Critère d'acceptation :** Les annonces avec une date de départ dans les 21 jours apparaissent en premier dans les résultats de recherche de l'acheteur, avec un badge "Départ imminent" visible, sans action supplémentaire de la vendeuse.

---

#### US-06 — Indicateur de prix de référence
**Story :** En tant qu'Awa (acheteuse), je veux voir une fourchette de prix indicative par type de meuble sur chaque annonce, afin de savoir si l'offre est juste sans avoir de repère de marché à Dakar.
**Priorité :** MUST
**Outil :** Bolt.new (affichage statique) + Dify (si calcul dynamique)
**Effort :** Faible
**Adresse :** Pain Reliever — Indicateur de prix de référence · Hypothèse I2
**Critère d'acceptation :** Chaque annonce affiche une mention du type "Prix moyen constaté à Dakar pour ce type de meuble : X – Y FCFA" basée sur une table de référence manuelle mise à jour par l'équipe Kaay Jënd.

---

#### US-07 — Paiement mobile sans compte bancaire sénégalais
**Story :** En tant qu'Amina (vendeuse), je veux recevoir un acompte de l'acheteur via un lien Wave ou Orange Money généré depuis la plateforme, afin de sécuriser la transaction avant ma date de départ sans avoir besoin d'un compte bancaire local.
**Priorité :** MUST
**Outil :** Bolt.new + Wave API ou lien de paiement Orange Money
**Effort :** Élevé
**Adresse :** Pain Reliever — Paiement mobile sans compte bancaire sénégalais · Contrainte MVP 6
**Critère d'acceptation :** La vendeuse peut générer un lien de paiement Wave ou Orange Money depuis son annonce, l'acheteur peut payer un acompte de 30 % via ce lien, et la vendeuse reçoit une confirmation de paiement sur son téléphone.

---

## User Stories SHOULD
*(À construire si le temps le permet en S3)*

#### US-08 — Notifications push "Départ imminent dans votre quartier"
**Story :** En tant qu'Awa (acheteuse), je veux recevoir une notification push quand un nouveau meuble correspondant à ma recherche est disponible dans mon quartier, afin d'être alertée sans avoir à consulter la plateforme chaque jour.
**Priorité :** SHOULD
**Outil :** Dify + notification push web ou SMS API
**Effort :** Élevé
**Adresse :** Pain Reliever — Fenêtre de vente prioritaire · Gain Creator — Marché cyclique prévisible
**Critère d'acceptation :** L'acheteuse reçoit une notification (push ou SMS) dans les 2 heures suivant la publication d'une annonce correspondant à ses critères de recherche et à son quartier.

---

#### US-09 — Mode délégation (mandataire de remise)
**Story :** En tant qu'Amina (vendeuse), je veux désigner un ami comme mandataire pour finaliser la remise du meuble après mon départ, afin de conclure la vente même si je ne suis plus à Dakar le jour de la remise.
**Priorité :** SHOULD
**Outil :** Bolt.new (formulaire de délégation) + QR code de transfert
**Effort :** Élevé
**Adresse :** Pain Reliever — Sécurité de la transaction · Contrainte MVP 6
**Critère d'acceptation :** La vendeuse peut renseigner le nom et le contact d'un mandataire depuis son profil, et l'acheteur reçoit les coordonnées du mandataire dès la confirmation du paiement de l'acompte.

---

#### US-10 — Galerie photo guidée avec cadres imposés
**Story :** En tant qu'Amina (vendeuse), je veux que l'application m'indique exactement quelles photos prendre (vue d'ensemble, défauts visibles, dimensions, état des pieds) avec des cadres guides à l'écran, afin de ne pas oublier d'angle important et de rassurer l'acheteur.
**Priorité :** SHOULD
**Outil :** Bolt.new (interface caméra guidée)
**Effort :** Élevé
**Adresse :** Pain Reliever — Galerie photo guidée en 4 angles · Contrainte MVP 3
**Critère d'acceptation :** L'interface de publication impose 4 étapes photo avec un libellé explicite pour chaque angle, bloque la publication si une photo est manquante, et compresse automatiquement les images pour fonctionner en 3G.

---

## User Stories COULD
*(Roadmap post-MVP)*

#### US-11 — Pack Arrivée (bundle à prix fixe)
**Story :** En tant qu'Awa (acheteuse), je veux pouvoir commander un bundle de meubles essentiels (lit, bureau, chaise, étagère) à prix fixe dès mon inscription, afin de m'installer sans avoir à chercher chaque meuble séparément.
**Priorité :** COULD
**Outil :** Bolt.new + logique de bundling
**Effort :** Élevé
**Adresse :** Gain Creator — Installation rapide et sereine · ⚠️ Hypothèse conditionnelle non validée en S3
**Critère d'acceptation :** ⚠️ À définir après validation de l'hypothèse C2 en interview S3 — construire uniquement si Awa confirme l'achat à distance sans visite physique.

---

#### US-12 — Système d'avis post-transaction
**Story :** En tant qu'Awa (acheteuse), je veux laisser un avis sur le vendeur et l'état du meuble après la transaction, afin d'aider les futurs acheteurs à choisir en confiance.
**Priorité :** COULD
**Outil :** Bolt.new
**Effort :** Moyen
**Adresse :** Gain Creator — Métriques de pilote actionnables · Hypothèse S1
**Critère d'acceptation :** L'acheteuse peut noter la transaction sur 5 et laisser un commentaire court dans les 48h suivant la confirmation de remise. La note est visible sur le profil du vendeur.

---

#### US-13 — Canal institutionnel (email de fin d'année)
**Story :** En tant que secrétariat pédagogique (partenaire), je veux recevoir un kit de communication clé en main (email + affiche) à envoyer aux étudiants étrangers en fin de cursus, afin de les orienter vers Kaay Jënd sans effort de rédaction.
**Priorité :** COULD
**Outil :** Autre (kit communication statique PDF + email)
**Effort :** Faible
**Adresse :** Gain Creator — Marché cyclique prévisible · Hypothèse S2
**Critère d'acceptation :** Le kit est envoyé à 3 institutions partenaires (UCAD, ESP, ISM) au moins 4 semaines avant le pic de départ de juin–juillet.

---

#### US-14 — Tableau de bord métriques pilote
**Story :** En tant que membre de l'équipe Kaay Jënd, je veux consulter en temps réel le nombre d'annonces publiées, le taux de conversion et le délai moyen de vente, afin de valider ou d'invalider les hypothèses du MVP à chaque cycle.
**Priorité :** COULD
**Outil :** Bolt.new (dashboard) + Dify (agrégation données)
**Effort :** Moyen
**Adresse :** Gain Creator — Métriques de pilote actionnables · Chapeau Bleu
**Critère d'acceptation :** Un tableau de bord interne affiche en temps réel : nombre d'annonces actives, nombre de contacts initiés, nombre de ventes confirmées et délai moyen annonce → vente confirmée.

---

## Sprint S3

**Semaine 1 — Fondations du MVP :**
US-01 (publication annonce) · US-02 (consultation par quartier) · US-03 (badge étudiant vérifié) · US-04 (contact vendeur WhatsApp)

**Semaine 2 — Mécanique de transmission et paiement :**
US-05 (transmission datée) · US-06 (indicateur prix de référence) · US-07 (paiement mobile Wave/OM)
Si avance de temps : US-10 (galerie photo guidée)

**Démo S6 — À démontrer obligatoirement en live :**
- US-01 : Publication d'une annonce en moins de 3 minutes sur Android
- US-02 : Recherche et filtrage d'annonces par quartier
- US-03 : Badge étudiant vérifié visible sur le profil
- US-05 : Badge "Départ imminent" sur une annonce avec date proche
- US-06 : Fourchette de prix de référence affichée sur une annonce
- US-07 : Génération et envoi d'un lien de paiement Wave ou Orange Money

---

### Récapitulatif des efforts S3

| Priorité | Nombre de US | Effort total estimé |
|---|---|---|
| MUST (à construire) | 7 | 3 faibles · 2 moyennes · 2 élevées |
| SHOULD (si temps) | 3 | 3 élevées |
| COULD (post-MVP) | 4 | 1 faible · 2 moyennes · 1 élevée |

---

*Kaay Jënd — Backlog S3 — Juin 2026*
