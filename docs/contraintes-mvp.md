# Contraintes MVP — Kaay Jënd

### Persona
Amina · 25 ans · Étudiante en Master · Dakar, Sénégal · Smartphone Android

---

## Contraintes Non Négociables

#### Contrainte 1
**Critère :** Le MVP DOIT permettre à un vendeur de publier une annonce en moins de 3 minutes, avec photos, prix et date de départ, depuis un smartphone Android en réseau 3G.
**Origine :** Chapeau Blanc — les étudiants bradent leurs meubles faute d'acheteurs identifiés à temps ; toute friction à la publication aggrave le problème de délai.
**Élimine :** Formulaires d'annonce longs, obligation de créer un compte complet avant de publier, téléchargement de photos en haute résolution, vérification d'identité préalable à la première annonce.

---

#### Contrainte 2
**Critère :** Le MVP DOIT être opérationnel et peuplé d'annonces actives au minimum 3 semaines avant chaque pic de départ (fin mai et fin novembre) pour ne pas arriver vide lors des fenêtres critiques.
**Origine :** Chapeau Blanc — les fins de cursus sont concentrées sur juin–juillet et décembre–janvier ; Chapeau Noir — la plateforme pourrait échouer à son propre pic d'usage si l'offre et la demande ne sont pas synchronisées à l'avance.
**Élimine :** Lancement en continu sans calendrier d'activation, stratégie d'acquisition utilisateurs non calée sur le calendrier académique, campagnes d'onboarding réactives plutôt que proactives.

---

#### Contrainte 3
**Critère :** Le MVP DOIT inclure un mécanisme minimal de vérification visuelle de l'état des meubles (galerie de photos guidée avec au moins 4 angles imposés : vue d'ensemble, défauts visibles, dimensions, état des pieds).
**Origine :** Chapeau Noir — sans preuve de qualité à distance, la méfiance des acheteurs reproduit exactement le problème actuel des groupes WhatsApp.
**Élimine :** Annonces texte seules, photo unique libre, descriptions non standardisées, système d'inspection physique tiers (trop lent et trop coûteux pour un MVP).

---

#### Contrainte 4
**Critère :** Le MVP DOIT être concentré géographiquement sur 1 à 2 quartiers ou campus de Dakar (ex. Mermoz, Fann, Liberté) pour atteindre la masse critique d'utilisateurs dès le premier cycle.
**Origine :** Chapeau Noir — le risque de dépendance au bouche-à-oreille est élevé ; si la masse critique n'est pas atteinte rapidement sur une zone précise, la plateforme reste vide.
**Élimine :** Couverture immédiate de tout Dakar, expansion multi-villes dès le lancement, ciblage diffus sans ancrage territorial.

---

#### Contrainte 5
**Critère :** Le MVP NE DOIT PAS reposer sur un modèle de reprise-revente (la plateforme achète les meubles pour les revendre) : il doit fonctionner en place de marché directe vendeur–acheteur.
**Origine :** Chapeau Noir — un modèle de reprise implique un stock physique, une trésorerie, une logistique et un risque financier incompatibles avec un MVP à ressources limitées.
**Élimine :** Entrepôt de stockage, acquisition de stock, gestion de livraison par la plateforme, pricing dynamique piloté par Kaay Jënd.

---

#### Contrainte 6
**Critère :** Le MVP DOIT intégrer un canal de paiement mobile accessible sans compte bancaire sénégalais (ex. lien de paiement Wave ou Orange Money) pour sécuriser les transactions sans exiger que le vendeur soit bancarisé localement.
**Origine :** Chapeau Blanc — les étudiants étrangers n'ont généralement pas de compte mobile money sénégalais actif ; Chapeau Noir — sans paiement sécurisé, la transaction échoue au moment critique de la remise.
**Élimine :** Paiement uniquement en espèces, virement bancaire, intégration de systèmes de paiement internationaux complexes (Stripe, PayPal) non adaptés au contexte local.

---

## Fonctionnalités Éliminées

- **Système de notation et d'avis détaillés** → éliminé parce qu'il nécessite un historique de transactions que le MVP n'aura pas lors des premières semaines ; remplacé par la vérification visuelle guidée (Contrainte 3).
- **Messagerie in-app complète** → éliminée parce qu'elle allonge le délai de développement et reproduit WhatsApp sans valeur ajoutée ; le contact initial peut passer par un numéro de téléphone masqué ou un lien WhatsApp direct.
- **Algorithme de recommandation et matching automatique** → éliminé parce qu'il requiert un volume de données que le MVP ne produira pas ; la géolocalisation par quartier suffit pour la première version.
- **Application iOS** → éliminée parce que le persona Amina et la majorité des étudiants étrangers à Dakar utilisent Android ; l'effort de développement iOS est injustifié pour le MVP.
- **Livraison organisée par la plateforme** → éliminée parce qu'elle implique une logistique opérationnelle (partenaires livreurs, assurance, délais) incompatible avec les fenêtres de vente de 2–3 semaines et les ressources d'un MVP.
- **Profil vendeur enrichi avec historique et badges** → éliminé parce que les vendeurs sont des étudiants en départ unique, pas des marchands récurrents ; la confiance repose sur la vérification du meuble, pas sur la réputation du vendeur.
- **Mode hors-ligne complet** → éliminé pour le MVP ; une optimisation 3G suffit pour la première version, le mode hors-ligne étant une amélioration post-validation.

---

## Critère de Validation Final

Le MVP est valide si et seulement si : au moins 70 % des meubles mis en vente sur la plateforme lors d'un cycle de départ (juin–juillet ou décembre–janvier) trouvent un acheteur confirmé avant la date de départ déclarée par le vendeur, sans que celui-ci ait eu besoin de baisser son prix de plus de 20 % par rapport à son prix initial.

---

*Kaay Jënd — Contraintes MVP — Juin 2026*
