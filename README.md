# 🔪 Qui a tué le Serveur ?

Jeu d'enquête interactif sur les **avantages et les limites des API REST**.

## Lancer le jeu
- Double-clique sur `index.html`, ou
- Dans VS Code : clic droit sur `index.html` → **Open with Live Server** (extension Live Server).

Une connexion internet permet de charger les polices (Bangers, Special Elite). Sans internet, le jeu fonctionne quand même.

## Déroulement
1. **Intro** : l'histoire du crash de FoodNow (bouton « Passer l'intro » pour aller vite).
2. **Interrogatoires** : 6 suspects × 3 questions. Chaque réponse ajoute un indice dans le carnet.
3. **Enveloppes** : 3 énigmes (logs, pièces à conviction, témoignages). Chaque énigme débloque la suivante.
4. **Accusation** : coupable, complice, arme, mobile, avantages, sauveur.
5. **Révélation** : verdict animé, score sur 12, débrief des avantages et des limites.

## Solution (pour l'animateur uniquement !)
- Coupable : **Polling** (pas de temps réel en REST)
- Complice : **Over-Fetching** (réponses de 2 Mo)
- Innocents avec alibi : **Le Cache** (mise en cache), **Stateless** (scalabilité)
- Sauveur : **WebSocket**
