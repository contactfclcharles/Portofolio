# Portfolio — à personnaliser

Ce dépôt contient un site portfolio prêt à l'emploi : un seul fichier `index.html`, qui
contient tout (HTML, CSS et JavaScript inclus dedans). Pas de framework, pas de dépendance
externe à installer — tu peux lire et modifier tout le code toi-même directement dans ce
fichier.

## 1. Personnaliser le contenu

Ton nom et ton email sont déjà en place. Il reste à remplacer ce qui est entre crochets `[...]` :

- Le paragraphe "À propos" (une astuce de rédaction est dans le commentaire juste au-dessus)
- Le projet phare : `[nom du site]`, `Contexte`, `Ce que j'ai fait` — dès que tu as le nom
  de domaine (tu m'as dit que tu l'achètes bientôt), remplace le bloc
  `<span class="project-link-pending">Bientôt en ligne</span>` par un vrai lien
  `<a href="https://ton-domaine.com" target="_blank" rel="noopener">Voir le site en ligne ↗</a>`
  et retire aussi la phrase "Nom de domaine en cours d'acquisition..." dans le `<p class="project-line">Résultat</p>`
- `[ton-pseudo]` (GitHub) et `[ton-profil]` (LinkedIn), dans le projet phare et dans "Contact"

Les deux cartes "Prochain projet" sont volontairement vides : garde-les comme rappel, ou
supprime-les si tu n'as qu'un seul projet pour l'instant. Ajoute une nouvelle carte en
copiant le bloc `<article class="project-card">...</article>` (pas la version "flagship")
du projet phare.

## Sur les techniques utilisées

Le site utilise des techniques de présentation qui font vraiment la différence pour un
recruteur : une accroche orientée bénéfice plutôt qu'une simple description, un badge de
disponibilité (signal de confiance immédiat), des chiffres précis plutôt que des adjectifs
vagues, une section "Pourquoi me faire confiance" écrite du point de vue de l'employeur, et
le projet phare mis en valeur visuellement avec une structure Contexte/Action/Résultat que
les recruteurs reconnaissent instinctivement.

Volontairement absent : faux témoignages, fausses statistiques, fausse urgence. Ce type de
procédé se retourne contre toi dès qu'un recruteur creuse un peu — mieux vaut une
présentation honnête, mais bien mise en scène.

## 2. Personnaliser le style (optionnel)

Tout le thème (couleurs, arrondis, largeur max) est défini tout en haut de la balise
`<style>` dans `index.html`, dans `:root { ... }`. Change `--accent` pour changer la couleur
d'accentuation, par exemple.

## 3. Voir le résultat en local

Ouvre simplement `index.html` dans ton navigateur (double-clic, ou clic droit → "Ouvrir avec").
Pas besoin de serveur, pas besoin d'autre fichier à côté — tout est inclus dans ce fichier
unique, donc impossible qu'un style ou un script "manquant" casse l'affichage.

## 4. Mettre le site en ligne gratuitement (GitHub Pages)

Ton dépôt `contactfclcharles/Portofolio` existe déjà sur GitHub — pas besoin de terminal ni
de `git`, tout se fait depuis le site web de GitHub :

1. Sur la page principale de ton dépôt, clique sur **"Add file" → "Upload files"**.
2. Glisse-dépose les 4 fichiers de ce dossier : `index.html`, `README.md`, `LICENSE.md` et
   `.gitignore`.
3. En bas de page, clique sur **"Commit changes"** pour les envoyer dans le dépôt.
4. Va dans **Settings → Pages** (dans le menu de gauche du dépôt) → sous "Build and
   deployment", choisis la branche `main` (dossier `/root`) → **Save**.
5. Après 1-2 minutes, ton site est en ligne à l'adresse :
   `https://contactfclcharles.github.io/Portofolio/`

Alternative tout aussi simple, sans compte GitHub : glisser-déposer le dossier sur
[netlify.com/drop](https://app.netlify.com/drop).

## 5. Idées pour la suite

- Ajouter une vraie photo/capture d'écran par projet.
- Ajouter un lien vers ton CV en PDF.
- Ajouter un nouveau projet dès que tu en termines un (voir section "Projets").
