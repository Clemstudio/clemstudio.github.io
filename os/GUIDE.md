# Atelier OS : mode d'emploi

## Où donner des ordres aux agents
Les agents vivent dans **Claude Code**, pas dans le chat claude.ai classique.

1. Ouvre https://claude.ai/code
2. Nouvelle session : choisis le dépôt `clemstudio/clemstudio.github.io`.
   Tant que la branche n'est pas fusionnée dans `main`, choisis la branche `claude/tiktok-video-shlpbj`.
3. Tape ta demande.

## Comment demander
| Je veux… | Je tape |
|---|---|
| Laisser le chef répartir | `/chef <mission>` |
| Trouver des clients | `/chef prospecte 3 garages à Seynod` |
| Auditer un site | `/chef audite le site exemple.fr` |
| Préparer un message pour un prospect | `/chef prépare le message pour Menuiserie des Cesardes` |
| Contenu TikTok / Insta | `/chef écris 3 scripts TikTok sur les erreurs des sites d'artisans` |
| Une fiche de cours | dépose le cours dans `os/cours/`, puis `/chef fais une fiche sur <sujet>` |
| Un quiz / calculs de doses | `/chef quiz de 10 questions sur <sujet>` |
| Mon planning | `/chef planning jusqu'aux partiels` |
| Parler à un agent précis | « Demande à Iris (auditeur-web) d'auditer exemple.fr » |
| Poser une question | Écris-la simplement, sans `/chef` |

## Qui fait quoi
- **Chef** : répartit les missions, met à jour le QG.
- **Malo** (`prospecteur`) : trouve des entreprises et rédige le message.
- **Iris** (`auditeur-web`) : audite un site, rapport + PDF.
- **Lou** (`redacteur-contenu`) : scripts TikTok et posts, rangés dans Notion Contenus.
- **Ana** (`tuteur-ifsi`) : fiches de révision à partir de tes cours.
- **Théo** (`quiz-ifsi`) : QCM, cas concrets, calculs de doses.
- **Jade** (`planificateur`) : planning révisions, stages, clients.

## Où voir les résultats
- **QG**, section « Atelier » : https://claude.ai/artifact/8g5GF3xUmpV8jQn8GqE9qr
- Nouvelles tâches : « Ta journée » du QG (Notion Tâches).
- Fichiers : `os/prospects/`, `os/audits/`, `os/fiches/`, `os/quiz/`, `os/contenus/`.

## Règles
- Les agents n'envoient jamais rien à un prospect : tu relis et tu envoies.
- Aucune donnée de patient ni info perso dans `os/` : le dépôt peut être public.
- La recherche web est limitée par le réseau de l'environnement (annuaires bloqués).
