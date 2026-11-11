# Kyara Bot pour Windows

Kyara Bot ouvre les packs gratuits disponibles et joue aux jeux solo de Kyara selon les réglages de chaque compte.

**Version actuelle : 1.6.7**

[Télécharger Kyara Bot 1.6.7 pour Windows](https://github.com/Abdou-Git/kyara-bot-releases/releases/download/v1.6.7/KyaraBotSetup-1.6.7.exe) · [Voir les nouveautés](https://github.com/Abdou-Git/kyara-bot-releases/releases/tag/v1.6.7)

Windows 10 ou 11 en 64 bits est nécessaire. L’installateur contient le navigateur, Node.js et Kyara Companion **1.4.5**. Il n’y a pas de commande à lancer, d’outil de développement à installer ou d’extension à charger manuellement pour un nouveau compte géré.

## Commencer

1. Télécharge puis installe `KyaraBotSetup-1.6.7.exe`
2. Lance Kyara Bot et clique sur **Ajouter un compte**
3. Connecte-toi normalement à Kyara dans la fenêtre qui s’ouvre, puis vérifie le compte dans le bot
4. Active les **Packs automatiques** si tu veux ouvrir les packs gratuits disponibles
5. Dans **Jeux solo**, sélectionne les jeux souhaités et active leur interrupteur

Les packs et les jeux s’activent séparément pour chaque compte. Chaque compte géré possède sa propre fenêtre et son propre profil. Garde le bot et les fenêtres Kyara ouverts pendant l’utilisation. La connexion initiale et les vérifications demandées par Kyara restent à faire manuellement.

## Jeux solo et tickets

Le bot propose douze jeux : Main du jour, Expédition, Les Trois Arcs, Main Kyara, Raid du jour, Raid Kyara, Kyara 21, Qui est-ce ?, Série express, Blind test, Mémoire et Le plus aimé. Tu peux modifier la sélection et mettre les jeux en pause pour chaque compte.

Le bouton **Ouvrir l’onglet du jeu** apparaît sur la carte du compte lorsqu’une partie est en cours, en pause ou à vérifier. Il affiche son onglet dans le bon profil ou le rouvre s’il a été fermé. Il ne lance pas de nouvelle partie, ne rejoue aucun coup et ne réactive pas les jeux à lui seul.

Si la partie reste au statut **Résultat à vérifier**, clique sur **Relancer les jeux**, juste à côté. Le bot ferme l’ancienne partie, attend la confirmation, puis réactive les jeux sélectionnés. L’historique, les choix de jeux, l’option de quota et les délais sont conservés. Le dernier coup incertain n’est pas rejoué et l’ancien résultat n’est pas confirmé. Si la fermeture échoue, les jeux restent en attente.

Par défaut, le bot termine la partie en cours puis attend lorsque le plafond de tickets du jour ou de la semaine est atteint. Il vérifie le quota toutes les cinq minutes et reprend quand les récompenses sont de nouveau disponibles.

Active **Couper le son des jeux** pour rendre silencieux les onglets de jeu du bot, y compris une partie déjà ouverte et les suivantes. Le réglage est enregistré par compte et reste disponible en pause. Tes autres onglets gardent leur son. Désactive-le pour rétablir le son du jeu. Si tu navigues vers une autre page dans cet onglet, Companion retire le silence qu’il avait appliqué.

Pour continuer à jouer au plafond, active **Jouer même au quota maximum**. Ce réglage est désactivé par défaut et ne donne pas de tickets supplémentaires. Si tu le désactives pendant une partie, le bot la termine avant de remettre les nouvelles parties en attente.

Les quiz reposent sur des heuristiques : les scores et les victoires ne sont pas garantis. Le blind test ne reconnaît pas l’audio. Les résultats affichés viennent de Kyara ; les délais et restrictions du site restent respectés.

## Mettre à jour

Dans le bot, ouvre **Réglages**, recherche une mise à jour, puis télécharge-la et installe-la. Tu peux aussi utiliser l’installateur ci-dessus. Les comptes, réglages, historiques et profils sont conservés dans `%LOCALAPPDATA%\KyaraBot`, séparément des fichiers de l’application.

L’application recherche aussi les nouvelles versions au lancement puis toutes les six heures. Le téléchargement et l’installation restent des actions explicites. Les mises à jour intégrées vérifient le manifeste signé et l’empreinte de l’installateur avant de l’exécuter.

## À savoir

L’installateur n’a pas de certificat Authenticode : Windows SmartScreen peut afficher un avertissement. La validation sur un Windows entièrement vierge reste à effectuer. La désinstallation conserve les données personnelles du bot.
