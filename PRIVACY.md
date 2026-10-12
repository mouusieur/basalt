# Politique de confidentialité de Basalt

*Dernière mise à jour : 12 octobre 2026. S'applique à Basalt 1.4.1 et versions suivantes.*

**En une phrase :** Basalt n'a pas de compte, pas de serveur qui collecte vos données, pas de publicité et pas de mouchard. Vos données restent sur votre PC. Les seules choses qui en sortent sont celles qu'il faut pour faire ce que vous demandez, et elles sont toutes listées ici.

## Ce que nous ne faisons jamais

- **Aucune télémétrie, aucune statistique d'usage**, aucun identifiant d'appareil ou de personne.
- **Aucune publicité**, aucune revente ni aucun partage de données à des fins commerciales.
- **Aucun compte obligatoire.** Les « comptes » de Basalt sont des profils locaux, qui ne quittent jamais votre PC.
- **Aucune synchronisation dans le cloud.** Basalt Labs ne reçoit ni votre historique, ni vos favoris, ni vos mots de passe, ni vos conversations avec Flint.

## Ce qui reste sur votre PC

Tout est rangé dans `%APPDATA%\Basalt`, sur votre ordinateur uniquement :

- historique, favoris, onglets ouverts, téléchargements, réglages ;
- **mots de passe** : dans un coffre chiffré (AES-256-GCM), qui n'existe que pour un compte protégé par un mot de passe. La clé est elle-même protégée par Windows (DPAPI) : le fichier copié sur un autre PC est inutilisable ;
- **étagère Flint** : les images et textes que vous gardez ;
- **rapports de plantage** en attente (voir plus bas), jamais envoyés sans votre accord.

Les **conversations avec Flint ne sont pas enregistrées** : elles disparaissent à la fermeture de Basalt. Les **fenêtres privées** n'écrivent ni historique ni cookies sur le disque.

Pour tout effacer : *Réglages → Shields & vie privée → Effacer les données de navigation*. Au moment de la désinstallation, Basalt vous propose aussi de supprimer ce dossier.

## Ce qui sort de votre PC, et pourquoi

### 1. Les sites que vous visitez
Comme avec n'importe quel navigateur, les sites reçoivent votre adresse IP et les informations techniques habituelles. **Basalt Shields** bloque par défaut les publicités et les traqueurs, avec les listes open source du projet Ghostery, mises à jour automatiquement depuis leur serveur. Vous pouvez aussi demander aux sites de ne pas vous suivre (« Do Not Track » / GPC).

### 2. La recherche Quarry
Quarry **n'a pas de serveur** : c'est votre PC qui interroge directement les sources, puis assemble les résultats. Votre recherche est envoyée à DuckDuckGo, Bing, Brave Search, YouTube, Wikipédia et, selon l'onglet choisi, Google Actualités, GitHub, Stack Overflow, npm ou MDN. Ces services voient la recherche et votre adresse IP, mais pas votre identité Basalt (il n'y en a pas).

- **Suggestions pendant la frappe** : DuckDuckGo, ou Bing en secours.
- **Réponses instantanées**, seulement si vous les demandez : conversion de devises (Frankfurter, ExchangeRate-API), météo (Open-Meteo, qui reçoit le nom de la ville), « mon IP » (ipify).
- **Météo de la page d'accueil** : Open-Meteo reçoit le nom de la ville choisie dans les réglages. Basalt n'utilise jamais votre position GPS pour ça.

### 3. Les icônes des sites
Pour afficher la petite icône de chaque site, Basalt la demande à DuckDuckGo (`icons.duckduckgo.com`, pour les onglets et les résultats) et à Google (`google.com/s2/favicons`, pour l'historique, les favoris et la page d'accueil). Ces services reçoivent donc le **nom de domaine** de ces sites, jamais l'adresse complète des pages.

### 4. Flint, l'assistant IA
Flint utilise des modèles d'IA **gratuits et sans compte**, hébergés par des services extérieurs. Basalt Labs ne reçoit et ne conserve **rien** de vos échanges.

**Ce qui est envoyé, uniquement quand vous utilisez Flint :**
- votre message et les derniers messages de la conversation ;
- **le texte de la page ouverte** (et le texte que vous avez sélectionné). C'est activé par défaut pour que Flint puisse « voir » ce que vous lisez. Une pastille 👁 indique la page partagée ; un clic dessus la désactive ;
- les images que vous lui montrez ;
- en **mode agent**, le contenu et des captures de l'onglet sur lequel il agit.

**Où ça part :** Kilo (kilo.ai), LLM7 (llm7.io), OVHcloud AI Endpoints (France) et AI Horde (aihorde.net). Basalt choisit automatiquement le modèle selon la tâche. Ces services voient votre adresse IP. **AI Horde est un réseau de bénévoles** : vos demandes y sont traitées par des ordinateurs de particuliers.

**Notre conseil :** ne confiez pas à Flint de mots de passe, de numéros de carte bancaire ou d'informations médicales. Flint refuse de taper un mot de passe, et l'agent vous demande votre accord avant les actions sensibles : achat, envoi d'un fichier, lecture du presse-papiers quand la tâche ne le concerne pas.

### 5. Les mises à jour
Toutes les 4 heures, Basalt télécharge un petit fichier signé qui annonce la dernière version. Il est hébergé sur Google Drive et GitHub, qui voient votre adresse IP. Aucune information sur vous ou votre usage n'est envoyée. Les mises à jour sont vérifiées par signature numérique avant d'être installées. Vous pouvez désactiver les mises à jour automatiques dans les réglages.

### 6. Vérification des mots de passe compromis
Si vous cliquez sur « Vérifier les fuites » dans le gestionnaire de mots de passe, Basalt interroge *Have I Been Pwned* de façon anonyme. Seuls les **5 premiers caractères de l'empreinte** de chaque mot de passe sont envoyés, jamais le mot de passe lui-même.

### 7. « Signaler un problème » et rapports de plantage
Quand Basalt plante, un rapport est **enregistré sur votre PC uniquement**. **Rien n'est envoyé tant que vous n'avez pas cliqué sur « Envoyer »**, et vous voyez avant le contenu exact du rapport.

Un rapport contient : votre description, la catégorie choisie, et, si vous laissez cochées ces options, des **informations techniques** (versions de Basalt et de Windows, quantité de mémoire, processeur, nombre d'onglets, quelques réglages) et les **plantages** (message d'erreur technique). Il ne contient **ni adresse de page, ni historique, ni nom d'utilisateur** : les chemins de fichiers sont anonymisés, les adresses web et e-mail retirées. Votre e-mail n'est joint que si vous l'écrivez vous-même, pour qu'on puisse vous répondre.

L'envoi passe par le service FormSubmit (formsubmit.co), qui transmet le rapport à la boîte mail de l'équipe. Vous pouvez aussi l'envoyer avec votre propre messagerie ou sur GitHub.

## Enfants
Basalt ne collecte aucune donnée personnelle, d'enfants ou d'adultes. Le contenu du web n'est pas filtré : la supervision d'un adulte est conseillée pour les plus jeunes.

## Vos droits
Comme nous ne détenons aucune donnée vous concernant, il n'y a rien à consulter ni à supprimer chez nous. Si vous nous avez écrit (rapport ou e-mail), demandez-nous la suppression de ce message à tout moment.

## Contact
Basalt Labs — **mouusieur@gmail.com**

Si cette politique change, la nouvelle version sera publiée avec la mise à jour correspondante, et sa date sera modifiée en haut de cette page.

---

# Basalt Privacy Policy

*Last updated: October 12, 2026. Applies to Basalt 1.4.1 and later.*

**In one sentence:** Basalt has no account, no server collecting your data, no ads and no tracker. Your data stays on your PC. The only things that leave it are what's needed to do what you ask, and they are all listed here.

## What we never do

- **No telemetry, no usage statistics**, no device or personal identifier.
- **No advertising**, no selling or sharing of data for commercial purposes.
- **No mandatory account.** Basalt "accounts" are local profiles that never leave your PC.
- **No cloud sync.** Basalt Labs never receives your history, bookmarks, passwords or Flint conversations.

## What stays on your PC

Everything lives in `%APPDATA%\Basalt`, on your computer only:

- history, bookmarks, open tabs, downloads, settings;
- **passwords**: in an encrypted vault (AES-256-GCM) that only exists for a password-protected account. The key is itself protected by Windows (DPAPI), so the file is useless if copied to another PC;
- **Flint shelf**: the images and texts you keep;
- pending **crash reports** (see below), never sent without your consent.

**Flint conversations are not saved**: they disappear when you close Basalt. **Private windows** write no history or cookies to disk.

To erase everything: *Settings → Shields & privacy → Clear browsing data*. When you uninstall, Basalt also offers to delete this folder.

## What leaves your PC, and why

### 1. The sites you visit
As with any browser, websites receive your IP address and the usual technical information. **Basalt Shields** blocks ads and trackers by default, using the open-source lists from the Ghostery project, updated automatically from their server. You can also ask sites not to track you (Do Not Track / GPC).

### 2. Quarry search
Quarry **has no server**: your own PC queries the sources directly, then assembles the results. Your query is sent to DuckDuckGo, Bing, Brave Search, YouTube, Wikipedia and, depending on the tab you choose, Google News, GitHub, Stack Overflow, npm or MDN. These services see the query and your IP address, but not your Basalt identity (there isn't one).

- **Suggestions while typing**: DuckDuckGo, with Bing as a fallback.
- **Instant answers**, only when you ask for them: currency conversion (Frankfurter, ExchangeRate-API), weather (Open-Meteo, which receives the city name), "my IP" (ipify).
- **Weather on the home page**: Open-Meteo receives the city chosen in the settings. Basalt never uses your GPS location for this.

### 3. Site icons
To show each site's small icon, Basalt asks DuckDuckGo (`icons.duckduckgo.com`, for tabs and results) and Google (`google.com/s2/favicons`, for history, bookmarks and the home page). These services therefore receive the **domain name** of those sites, never the full page addresses.

### 4. Flint, the AI assistant
Flint uses **free AI models that need no account**, hosted by outside services. Basalt Labs receives and keeps **nothing** of your exchanges.

**What is sent, only when you use Flint:**
- your message and the latest messages of the conversation;
- **the text of the open page** (and any text you selected). This is on by default so Flint can "see" what you are reading. A 👁 chip shows the shared page; click it to turn this off;
- the images you show it;
- in **agent mode**, the content and screenshots of the tab it is working on.

**Where it goes:** Kilo (kilo.ai), LLM7 (llm7.io), OVHcloud AI Endpoints (France) and AI Horde (aihorde.net). Basalt picks the model automatically depending on the task. These services see your IP address. **AI Horde is a volunteer network**: your requests are processed on private individuals' computers.

**Our advice:** don't give Flint passwords, card numbers or medical information. Flint refuses to type passwords, and the agent asks for your consent before sensitive actions: purchases, uploading a file, reading your clipboard when the task isn't about it.

### 5. Updates
Every 4 hours, Basalt downloads a small signed file announcing the latest version. It is hosted on Google Drive and GitHub, which see your IP address. No information about you or your usage is sent. Updates are checked with a digital signature before they are installed. You can turn off automatic updates in the settings.

### 6. Breached password check
If you click "Check for leaks" in the password manager, Basalt anonymously asks *Have I Been Pwned*. Only the **first 5 characters of each password's hash** are sent, never the password itself.

### 7. "Report a problem" and crash reports
When Basalt crashes, a report is **saved on your PC only**. **Nothing is sent until you click "Send"**, and you see the exact content of the report first.

A report contains: your description, the category you chose, and, if you leave these options checked, **technical information** (Basalt and Windows versions, amount of memory, processor, number of tabs, a few settings) and the **crashes** (technical error message). It contains **no page addresses, no history and no user name**: file paths are anonymized, and web and email addresses are removed. Your email is only included if you type it yourself, so we can reply.

Reports are sent through the FormSubmit service (formsubmit.co), which forwards them to the team's mailbox. You can also send them with your own email app or on GitHub.

## Children
Basalt collects no personal data from children or adults. Web content isn't filtered: adult supervision is recommended for young children.

## Your rights
Since we hold no data about you, there is nothing to view or delete on our side. If you wrote to us (report or email), you can ask us to delete that message at any time.

## Contact
Basalt Labs — **mouusieur@gmail.com**

If this policy changes, the new version will ship with the matching update, and the date at the top of this page will change.
