# Mes sites — règles

Hub (lien de la bio Instagram) qui présente les applis de Théo. Répondre en français, court et simple. Théo veut une page **simple mais cool, façon hub** : pas de captures d'écran des applis, pas de surcharge.

- Servi sur `theo1010-dev.github.io/Mes-sites/`, le même domaine que Mon Frigo, Mon Budget et Ma stratégie.
  → **Jamais de service worker**, jamais de code qui touche au stockage (localStorage, IndexedDB, caches) : ça pourrait casser les applis ou leurs données.
- Ordre des cartes voulu par Théo : PotoStick, Mon Frigo, Mon Budget, Ma stratégie. Pas de trait sous le titre.
- Les cartes ouvrent l'appli dans un nouvel onglet (`target="_blank"`) : le hub reste ouvert, et le lien Insta ramène toujours au hub.
- Ne JAMAIS mettre de domaine perso sur un dépôt `Theo1010-dev.github.io` : toutes les applis changeraient d'adresse et perdraient leurs données.
- Un seul fichier `index.html` (CSS dans la page), polices dans `fonts/` (OFL), icônes 192 px dans `icons/`, `og.png` = aperçu quand on partage le lien.
- Ajouter une appli : un `<li><a class="card …">` + une classe de couleurs (--bg, --ink, --muted, --ring, --tag-bg, --tag-ink, --btn, --on-btn) + son icône.
- Vérifier à 320 et 390 px (aucun débordement), puis pousser sur `main`.
