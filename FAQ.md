# Questions fréquentes

## Installation

### Basalt est-il vraiment gratuit ?
Oui. Pas de publicité, pas d'abonnement, pas de compte à créer, pas de version « Pro ». Flint, l'assistant IA, est gratuit lui aussi, et sans clé.

### Windows affiche « Windows a protégé votre ordinateur ». Est-ce dangereux ?
Non. Ce message (SmartScreen) s'affiche pour les nouveaux logiciels qui n'ont pas encore de certificat de signature payant ou de réputation suffisante. Cliquez sur **Informations complémentaires**, puis sur **Exécuter quand même**. Vous pouvez vérifier que le fichier n'a pas été modifié : son empreinte SHA-256 est publiée sur la page de téléchargement GitHub.

### Mon antivirus signale Basalt. Que faire ?
C'est un **faux positif** fréquent pour les logiciels récents non signés. Basalt ne contient ni publicité, ni logiciel tiers, ni mouchard. Vous pouvez analyser l'installateur sur [VirusTotal](https://www.virustotal.com) et nous signaler le nom de l'antivirus : nous demanderons une correction à son éditeur.

### Faut-il des droits administrateur ?
Non. Basalt s'installe pour votre session Windows uniquement, dans votre dossier utilisateur.

### Quelle configuration faut-il ?
Windows 10 ou 11 en 64 bits. Basalt est pensé pour les PC modestes : 4 Go de mémoire suffisent. Sur un vieux PC, activez **Réglages → Performance → Mode éco** : moins d'animations, onglets mis en veille plus vite, moins de processus.

### Comment désinstaller Basalt ?
*Paramètres Windows → Applications → Basalt → Désinstaller*. Basalt vous demande si vous voulez aussi supprimer vos données (historique, favoris, etc.).

## Utilisation

### Comment récupérer mes favoris de Chrome ou Edge ?
*Réglages → Général → Importer depuis un autre navigateur*. Basalt importe les favoris et l'historique récent de Chrome, Edge, Brave, Vivaldi, Opera, Opera GX et Arc. Les mots de passe ne sont pas importés automatiquement.

### Comment faire de Basalt mon navigateur par défaut ?
*Réglages → Général → Navigateur par défaut → Définir par défaut*, puis choisissez Basalt dans la fenêtre de Windows qui s'ouvre.

### Un site s'affiche mal ou ne fonctionne pas.
Le bloqueur (Basalt Shields) est parfois trop zélé. Cliquez sur le **bouclier** à gauche de l'adresse et désactivez Shields **pour ce site uniquement**. Si le problème continue, signalez-le-nous avec *Menu → Signaler un problème*.

### Google refuse ma connexion (« Ce navigateur n'est peut-être pas sécurisé »).
Basalt contourne ce blocage automatiquement. Si le message apparaît quand même, fermez l'onglet, rouvrez la page de connexion et réessayez.

### Où sont mes mots de passe ? Sont-ils en sécurité ?
Le gestionnaire de mots de passe nécessite un **compte protégé par mot de passe** (*Réglages → Comptes · sécurité*). Les mots de passe sont alors chiffrés sur votre PC et ne sont jamais envoyés nulle part. Un bilan de santé repère les mots de passe faibles, réutilisés ou apparus dans des fuites.

### Puis-je installer des extensions Chrome ?
Pas pour l'instant. Basalt intègre déjà l'essentiel : bloqueur de publicités et de traqueurs, gestionnaire de mots de passe, mode lecture, capture d'écran, écran partagé, onglets verticaux, panneau développeur et Flint.

### Quels raccourcis connaître ?
- **Ctrl K** : palette de commandes (tout est accessible au clavier)
- **Ctrl E** : ouvrir Flint
- **Ctrl Maj X** : capture d'écran
- **Ctrl Maj S** : écran partagé
- **F1** : cette aide

## Quarry, le moteur de recherche

### Qu'est-ce que Quarry ?
Le moteur de recherche intégré à Basalt : web, images, vidéos, actualités, shopping et développeurs, sans publicité. Il n'a **pas de serveur** : votre PC interroge directement plusieurs sources (DuckDuckGo, Bing, Brave Search, YouTube, Wikipédia…) et assemble les résultats.

### Puis-je utiliser Google à la place ?
Oui : *Réglages → Recherche · Quarry*. Vous pouvez choisir un autre moteur par défaut.

## Flint, l'assistant IA

### Faut-il une clé, un compte ou un abonnement ?
Non, rien de tout ça. Flint utilise des modèles d'IA gratuits et choisit automatiquement le plus adapté : rapide pour une question simple, le plus puissant pour une grosse tâche, un spécialiste pour le code.

### Pourquoi Flint est-il parfois lent, ou dit que les modèles sont occupés ?
Les modèles gratuits sont partagés entre beaucoup d'utilisateurs et ont des quotas. Flint passe automatiquement à un autre modèle quand l'un est saturé. Si tous le sont, réessayez une minute plus tard.

### Que voit Flint de mes pages ?
Par défaut, Flint lit **le texte de la page ouverte** pour pouvoir en parler. La pastille 👁 en bas de Flint indique quelle page est partagée ; un clic dessus la désactive. Les conversations ne sont pas enregistrées. Plus de détails dans la page *Confidentialité*.

### Que peut faire le mode agent ?
Agir dans un onglet à votre place : chercher, cliquer, remplir un formulaire, trouver et copier des images, résumer une vidéo avec ses moments clés, lire des tableaux, envoyer un fichier dans un site, etc. Vous voyez chaque étape et pouvez l'arrêter à tout moment. Il ne tape **jamais** de mot de passe et vous demande votre accord avant les actions sensibles (*Réglages → Flint · copilote IA → Demander avant les actions sensibles*).

### Qu'est-ce que l'étagère Flint ?
L'endroit où Flint (ou vous, avec un clic droit sur une image → *Garder sur l’étagère Flint*) range les images et textes gardés. Depuis l'étagère, vous pouvez les copier, les enregistrer, les glisser dans un autre logiciel ou les envoyer à Flint.

## Mises à jour et aide

### Comment fonctionnent les mises à jour ?
Automatiquement : Basalt télécharge la nouvelle version en arrière-plan (souvent quelques Mo), vérifie sa signature numérique, puis l'applique au prochain redémarrage. Si une version ne démarre pas, Basalt revient tout seul à la précédente.

### Comment signaler un bug ou proposer une idée ?
*Menu (⋯) → Signaler un problème*, ou la touche **F1** → *Signaler un problème*. Vous voyez exactement ce qui est envoyé avant de cliquer sur « Envoyer ». Vous pouvez aussi écrire à **mouusieur@gmail.com**.

---

# Frequently asked questions

## Installation

### Is Basalt really free?
Yes. No ads, no subscription, no account to create, no "Pro" edition. Flint, the AI assistant, is free too, and needs no key.

### Windows says "Windows protected your PC". Is it dangerous?
No. This message (SmartScreen) appears for new software that doesn't yet have a paid code-signing certificate or enough reputation. Click **More info**, then **Run anyway**. You can check that the file hasn't been tampered with: its SHA-256 hash is published on the GitHub download page.

### My antivirus flags Basalt. What should I do?
It's a common **false positive** for new, unsigned software. Basalt contains no ads, no bundled third-party software and no tracker. You can scan the installer on [VirusTotal](https://www.virustotal.com) and tell us which antivirus flagged it: we'll ask its vendor to fix it.

### Do I need administrator rights?
No. Basalt installs for your Windows user only, in your user folder.

### What are the system requirements?
Windows 10 or 11, 64-bit. Basalt is designed for modest PCs: 4 GB of memory is enough. On an old PC, turn on **Settings → Performance → Eco mode**: fewer animations, tabs put to sleep sooner, fewer processes.

### How do I uninstall Basalt?
*Windows Settings → Apps → Basalt → Uninstall*. Basalt asks whether you also want to delete your data (history, bookmarks, etc.).

## Using Basalt

### How do I bring over my bookmarks from Chrome or Edge?
*Settings → General → Import from another browser*. Basalt imports bookmarks and recent history from Chrome, Edge, Brave, Vivaldi, Opera, Opera GX and Arc. Passwords are not imported automatically.

### How do I make Basalt my default browser?
*Settings → General → Default browser → Make default*, then pick Basalt in the Windows window that opens.

### A site looks broken or doesn't work.
The blocker (Basalt Shields) is sometimes too strict. Click the **shield** left of the address and turn Shields off **for that site only**. If the problem persists, tell us with *Menu → Report a problem*.

### Google refuses my sign-in ("This browser may not be secure").
Basalt works around this block automatically. If you still see the message, close the tab, reopen the sign-in page and try again.

### Where are my passwords? Are they safe?
The password manager needs a **password-protected account** (*Settings → Accounts · security*). Your passwords are then encrypted on your PC and never sent anywhere. A health check finds weak, reused or leaked passwords.

### Can I install Chrome extensions?
Not yet. Basalt already includes the essentials: ad and tracker blocker, password manager, reader mode, screenshots, split view, vertical tabs, developer panel and Flint.

### Which shortcuts should I know?
- **Ctrl K**: command palette (everything is reachable from the keyboard)
- **Ctrl E**: open Flint
- **Ctrl Shift X**: screenshot
- **Ctrl Shift S**: split view
- **F1**: this help

## Quarry, the search engine

### What is Quarry?
Basalt's built-in search engine: web, images, videos, news, shopping and developer results, with no ads. It has **no server**: your PC queries several sources directly (DuckDuckGo, Bing, Brave Search, YouTube, Wikipedia…) and assembles the results.

### Can I use Google instead?
Yes: *Settings → Search · Quarry*. You can choose another default search engine.

## Flint, the AI assistant

### Do I need a key, an account or a subscription?
No, none of them. Flint uses free AI models and automatically picks the best fit: a fast one for a simple question, the most powerful for a big task, a specialist for code.

### Why is Flint sometimes slow, or says models are busy?
Free models are shared by many users and have quotas. Flint automatically switches to another model when one is overloaded. If they all are, try again a minute later.

### What does Flint see of my pages?
By default, Flint reads **the text of the open page** so it can talk about it. The 👁 chip at the bottom of Flint shows which page is shared; click it to turn this off. Conversations are not saved. More details on the *Privacy* page.

### What can agent mode do?
Act in a tab for you: search, click, fill in a form, find and copy images, summarize a video with its key moments, read tables, upload a file to a site, and more. You see every step and can stop it at any time. It **never** types passwords and asks for your consent before sensitive actions (*Settings → Flint · AI copilot → Ask before sensitive actions*).

### What is the Flint shelf?
The place where Flint (or you, by right-clicking an image → *Keep on the Flint shelf*) stores kept images and texts. From the shelf you can copy them, save them, drag them into another app or send them to Flint.

## Updates and help

### How do updates work?
Automatically: Basalt downloads the new version in the background (often just a few MB), checks its digital signature, then applies it at the next restart. If a version fails to start, Basalt goes back to the previous one by itself.

### How do I report a bug or suggest an idea?
*Menu (⋯) → Report a problem*, or press **F1** → *Report a problem*. You see exactly what is sent before clicking "Send". You can also write to **mouusieur@gmail.com**.
