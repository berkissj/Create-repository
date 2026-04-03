# MÉMO FRAMEWORK RICE / RCTCF
## La méthode pour des prompts puissants — Fiche à garder sur votre bureau

---

## LE FRAMEWORK EN UN COUP D'OEIL

```
┌─────────────────────────────────────────────────────┐
│                                                     │
│   R — RÔLE         Qui est l'IA pour cette tâche ?  │
│   I — INSTRUCTION  Que doit-elle faire exactement ?  │
│   C — CONTEXTE     Quel est le contexte à connaître ?│
│   E — EXEMPLE      Quel format/résultat j'attends ?  │
│                                                     │
└─────────────────────────────────────────────────────┘
```

**Variante étendue : RCTCF**
- **R** — Rôle
- **C** — Contexte
- **T** — Tâche (l'instruction précise)
- **C** — Contraintes (limites, format, longueur, ton)
- **F** — Format (comment structurer le résultat)

---

## LES 4 ÉTAPES DÉTAILLÉES

### R — RÔLE
Donnez une identité à l'IA. Plus le rôle est précis, meilleur est le résultat.

| Faible | Fort |
|--------|------|
| "Aide-moi à écrire" | "Tu es un directeur marketing avec 15 ans d'expérience en Afrique de l'Ouest, spécialisé dans le B2B" |
| "Analyse ce document" | "Tu es un analyste financier senior, rigoureux et orienté données" |

**Astuce** : Ajoutez l'expertise, le ton, et le style souhaité dans le rôle.

---

### I — INSTRUCTION
Soyez précis sur ce que vous voulez. Une instruction vague = un résultat vague.

| Faible | Fort |
|--------|------|
| "Écris un email" | "Rédige un email de relance à un client qui n'a pas répondu depuis 2 semaines. L'email doit être courtois mais ferme, et proposer un nouveau rendez-vous" |
| "Fais un résumé" | "Résume ce document en 5 points clés maximum, en mettant en avant les chiffres importants et les recommandations d'action" |

**Astuce** : Utilisez des verbes d'action précis : "rédige", "analyse", "compare", "structure", "identifie", "propose".

---

### C — CONTEXTE
Donnez à l'IA les informations dont elle a besoin pour bien répondre.

**Ce qu'il faut inclure :**
- Qui est le destinataire ? (patron, client, équipe, prospect...)
- Quelle est la situation ? (urgence, routine, conflit, lancement...)
- Quel est l'historique ? (première fois, relance, suivi...)
- Quel est votre secteur/métier ?
- Y a-t-il des contraintes particulières ?

| Faible | Fort |
|--------|------|
| "Écris un rapport" | "Je suis directeur commercial d'une banque en Côte d'Ivoire. Mon DG me demande un rapport sur les performances du T1. Nous avons dépassé nos objectifs de 12% mais le taux de rétention a baissé de 5%." |

---

### E — EXEMPLE
Montrez à l'IA le format ou le style de résultat que vous attendez.

**3 façons de donner un exemple :**
1. **Un modèle** : "Voici un exemple d'email que j'ai écrit la dernière fois : [coller l'email]. Écris dans le même style."
2. **Un format** : "Structure ta réponse ainsi : 1) Contexte (2 lignes) 2) Analyse (5 points) 3) Recommandations (3 actions)"
3. **Un ton** : "Ton professionnel mais accessible, comme si tu expliquais à un collègue intelligent qui ne connaît pas le sujet"

---

## CHECKLIST : MON PROMPT EST-IL BON ?

Avant d'envoyer votre prompt, vérifiez ces 7 critères :

- [ ] **1. Rôle défini** — J'ai précisé QUI est l'IA pour cette tâche
- [ ] **2. Instruction claire** — J'ai utilisé un verbe d'action précis
- [ ] **3. Contexte fourni** — J'ai donné les informations nécessaires
- [ ] **4. Résultat attendu** — J'ai décrit ce que je veux obtenir
- [ ] **5. Format précisé** — J'ai indiqué comment structurer la réponse
- [ ] **6. Contraintes posées** — J'ai précisé la longueur, le ton, les limites
- [ ] **7. Pas d'ambiguïté** — Un collègue comprendrait ma demande sans poser de question

**Règle d'or** : Si votre prompt fait moins de 3 lignes, il est probablement trop vague.

---

## 5 EXEMPLES AVANT / APRÈS

### Exemple 1 — Email professionnel

**AVANT (prompt basique)** :
> Écris un email à mon client

**APRÈS (prompt RICE)** :
> **Rôle** : Tu es mon assistant de communication professionnelle. Tu écris de manière courtoise, directe et orientée solution.
>
> **Instruction** : Rédige un email de relance à un client qui devait valider un devis il y a 10 jours et qui n'a pas répondu.
>
> **Contexte** : Le client est le DRH d'une entreprise de 200 personnes au Cameroun. Le devis concerne une formation en management pour 15 managers. Montant : 4 500 000 FCFA. On a eu un bon échange téléphonique il y a 3 semaines.
>
> **Exemple de ton** : Professionnel mais chaleureux. Pas de pression agressive. Proposer un court appel pour répondre à d'éventuelles questions.

---

### Exemple 2 — Analyse de données

**AVANT** :
> Analyse ces chiffres de vente

**APRÈS** :
> **Rôle** : Tu es un analyste commercial expérimenté.
>
> **Instruction** : Analyse les données de vente ci-dessous et identifie : (1) les 3 produits les plus performants, (2) les tendances sur les 3 derniers mois, (3) les zones géographiques à fort potentiel, (4) 3 recommandations d'action.
>
> **Contexte** : Je suis directeur commercial d'une entreprise agroalimentaire en Afrique de l'Ouest. Voici les données : [COLLER LES DONNÉES]
>
> **Format** : Présente ton analyse en sections numérotées avec des bullet points. Termine par un tableau récapitulatif.

---

### Exemple 3 — Présentation PowerPoint

**AVANT** :
> Fais-moi un PowerPoint sur l'IA

**APRÈS** :
> **Rôle** : Tu es un consultant en stratégie digitale qui prépare des présentations pour des comités de direction.
>
> **Instruction** : Crée le plan détaillé d'une présentation de 15 slides sur "Pourquoi et comment intégrer l'IA dans notre entreprise".
>
> **Contexte** : Public = le comité de direction (DG, DRH, DAF, Directeur commercial) d'une banque de 500 employés. Ils sont sceptiques mais curieux. Budget disponible : limité.
>
> **Format** : Pour chaque slide, donne : le titre, les 3-4 bullet points, et une suggestion de visuel. Commence par un chiffre choc. Termine par 3 actions concrètes à lancer dès lundi.

---

### Exemple 4 — Résumé de document

**AVANT** :
> Résume ce document

**APRÈS** :
> **Rôle** : Tu es un assistant exécutif habitué à préparer des briefs pour des dirigeants pressés.
>
> **Instruction** : Résume ce rapport en un brief exécutif de maximum 300 mots.
>
> **Contexte** : Ce rapport sera lu par le DG qui a 5 minutes. Il veut savoir : (1) les conclusions principales, (2) les chiffres clés, (3) ce qu'il doit décider.
>
> **Format** : 3 sections — "En bref" (2 phrases), "Chiffres clés" (3-5 données), "Décision requise" (1-2 phrases). Pas de jargon.
>
> [COLLER LE DOCUMENT]

---

### Exemple 5 — Brainstorming

**AVANT** :
> Donne-moi des idées pour améliorer les ventes

**APRÈS** :
> **Rôle** : Tu es un consultant en stratégie commerciale avec une expertise en marché africain.
>
> **Instruction** : Génère 10 idées concrètes et actionnables pour augmenter les ventes de notre entreprise de 20% en 6 mois.
>
> **Contexte** : Entreprise de formation professionnelle au Sénégal. CA actuel : 25M FCFA/mois. Produits : formations en management et leadership. Canaux actuels : bouche-à-oreille + webinaires. Base email : 15 000 contacts peu exploitée. Équipe marketing : 2 personnes.
>
> **Contraintes** : Budget marketing limité à 2M FCFA/mois. Pas de force de vente terrain. Les idées doivent être réalisables avec une petite équipe.
>
> **Format** : Pour chaque idée, donne : le titre, la description en 2 lignes, le coût estimé, et l'impact attendu (faible/moyen/fort).

---

## RÈGLES D'OR DU PROMPTING

1. **Itérez** — Le premier résultat n'est jamais parfait. Affinez en 2-3 échanges.
2. **Soyez spécifique** — "Un rapport de 500 mots" > "Un rapport court"
3. **Donnez le contexte métier** — L'IA ne connaît pas votre entreprise, dites-lui.
4. **Montrez un exemple** — Un exemple vaut mille instructions.
5. **Corrigez en direct** — "C'est bien mais le ton est trop formel, rends-le plus accessible"
6. **Sauvegardez vos bons prompts** — Créez votre bibliothèque personnelle.
7. **Ne faites jamais confiance aveuglément** — Vérifiez toujours les faits et les chiffres.
