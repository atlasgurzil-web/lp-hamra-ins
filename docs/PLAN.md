# Plan : Landing Page Mobile-First • Section Échecs — Hamra Annaba

> PRD source : docs/PRD.md

## Décisions architecturales

- **Architecture :** Single-Page moderne et ultra-rapide (HTML5 sémantique + Tailwind CSS + Lucide Icons SVG inline). Zéro dépendance lourde, chargement instantané (< 1 seconde) optimisé pour les réseaux mobiles algériens (3G/4G).
- **Canal d'action principal :** Lien direct tel:0669546680 ouvrant l'application Téléphone en 1 tap.
- **Canal d'action secondaire :** Lien direct sms:0669546680 avec message pré-rempli.
- **Charte visuelle & Design Tokens :**
  - Rouge officiel Hamra Annaba (#E00613, nuances #B91C1C au hover, #EF4444 en accent)
  - Blanc pur (#FFFFFF) et fond neutre clair (#F8FAFC, #F1F5F9)
  - Contrastes profonds Slate (#0F172A, #1E293B) garantissant un ratio WCAG AAA > 12:1
  - Typographie : Sans-serif athlétique géométrique moderne (Plus Jakarta Sans / Inter)
  - Asset officiel : assets/images/logo-hamra.png
  - Sticky CTA mobile : Barre de conversion en verre dépoli (backdrop-blur-md bg-white/95 border-t border-slate-200) avec tap target minimum de 52px.

---

## Phase 1 : Cœur de conversion & Hero mobile-first

**User stories** : US-1, US-2, US-3

### Ce qu'on livre

L'en-tête officiel et le Hero haute conversion. Dès l'ouverture sur smartphone, le visiteur voit le logo authentique du Hamra Annaba 1944 avec son nom bilingue (*حمراء عنابة*), l'offre claire (Section Échecs, tous âges, 2 000 DA/mois, créneaux mardi dès 17h et samedi dès 10h, Tennis Club d'Annaba face au Consulat de France), et deux boutons d'action immédiate (Appel direct vers Monsieur Bentboula au 0669 54 66 80 et SMS pré-rempli).

### Critères d'acceptation

- [ ] Le logo officiel Hamra Annaba s'affiche de manière nette et centrée/alignée dans l'en-tête.
- [ ] Le tarif de 2 000 DA/mois, les deux créneaux et le lieu TCA sont lisibles au premier coup d'œil sans scroll nécessaire.
- [ ] Un clic sur le bouton principal déclenche immédiatement l'appel vers le 0669 54 66 80.
- [ ] Un clic sur le bouton SMS ouvre l'application SMS avec le message pré-rempli.
- [ ] La page est 100% responsive sur mobile (360px à 430px).

## Bloquée par

Aucune — démarrable immédiatement.

---

## Phase 2 : Pôles d'entraînement & Différenciation (Enfants vs Ados/Adultes)

**User stories** : US-4, US-5

### Ce qu'on livre

La section « Pourquoi nous rejoindre » structurée en deux cartes visuelles distinctes à fort impact :
1. Pôle Enfants : concentration, réflexion, stratégie, plaisir d'apprendre et tournois.
2. Pôle Adolescents & Adultes : jeu régulier, progression à son niveau, adversaires motivés, tournois et vie de club.

### Critères d'acceptation

- [ ] Les bénéfices enfants et adultes sont immédiatement compréhensibles et différenciés.
- [ ] Utilisation exclusive d'icônes vectorielles SVG soignées (zéro emoji).
- [ ] Les micro-interactions (hover, active tap) sont fluides et tactiles.

## Bloquée par

- Phase 1

---

## Phase 3 : Horaires détaillés, Localisation au TCA & Vie du Club

**User stories** : US-6

### Ce qu'on livre

La section détaillée des cours (Mardi 17h00, Samedi 10h00 avec Monsieur Bentboula), le repère géographique précis au Tennis Club d'Annaba (TCA, en face du Consulat de France avec lien d'itinéraire Maps), et la mise en valeur des tournois mensuels réguliers dans un design vectoriel sportif sans fausse photo.

### Critères d'acceptation

- [ ] Les jours et heures sont mis en valeur dans des cartes d'horaires claires.
- [ ] L'adresse TCA face Consulat de France est accompagnée d'un repère visuel clair.
- [ ] La fréquence des tournois (quasiment tous les mois) et la vie de club sont valorisées sans afficher de fausse photo.

## Bloquée par

- Phase 2

---

## Phase 4 : Parcours d'inscription simplifié & Sticky Action Bar Mobile

**User stories** : US-2, US-6, US-7

### Ce qu'on livre

La section finale d'inscription résumée en 3 étapes sans friction (Contacter Monsieur Bentboula, Préparer extrait de naissance + photos, Venir à la prochaine séance) avec grand rappel du numéro, ainsi que la barre d'action mobile fixe (Sticky Bottom Bar) avec bouton d'appel direct et SMS visible en continu lors du défilement.

### Critères d'acceptation

- [ ] Les pièces d'inscription (extrait de naissance + photos) sont immédiatement repérables.
- [ ] Le bouton d'appel final grand format permet de téléphoner directement.
- [ ] La barre d'action fixe en bas d'écran reste visible sur mobile sans masquer le contenu (padding inférieur adapté).
- [ ] Audit visuel validé (WCAG AA, fluidité 60fps, aucun overflow horizontal).

## Bloquée par

- Phase 3
