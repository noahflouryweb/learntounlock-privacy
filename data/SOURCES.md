# Dictionnaire anglais → français de LearnToUnlock

**Version en service : `dict-en-fr-2.tsv.gz`** (16/11/2026), fabriquée par `scripts/build-dict2.py`. Elle reclasse les
traductions à partir des tableaux de traduction des entrées anglaises du Wiktionnaire (un sens par ligne), extraits par
Matthias Buchmeier et repris du dépôt GitHub `open-dsl-dict/wiktionary-dict` (CC BY-SA 3.0 et GFDL) ; définitions,
synonymes et phrases d'exemple viennent de la version 1. Sur les 463 mots seuls de la banque, la première traduction
est celle de la banque dans 64 % des cas (54 % pour la version 1), et l'une des trois premières dans 77 % (69 %).
La version 1 ci-dessous reste dans le dossier : elle sert d'entrée à la version 2.


`dict-en-fr-1.tsv.gz` : environ 19 500 mots anglais parmi les plus fréquents, avec leurs traductions françaises
(de la plus courante à la plus rare), une définition anglaise, des synonymes et, pour certains, des phrases d'exemple
traduites. Téléchargé par l'app au premier usage (Mes cours › un paquet › Chercher), puis utilisé hors ligne.

Fabriqué par `scripts/build-dict.py` (dépôt de l'app) à partir de :

- **Wiktionary** (Wiktionnaire en anglais, entrées françaises), extrait par kaikki.org (wiktextract) :
  traductions (gloses inversées) et phrases d'exemple. Licence CC BY-SA 4.0 et GFDL.
  https://kaikki.org — https://en.wiktionary.org
- **Lexique 3** : fréquence des mots français, pour classer les traductions. Licence CC BY-SA 4.0. http://www.lexique.org
- **wordfreq** : liste des mots anglais les plus fréquents. Données sous licence CC BY-SA 4.0.
  https://github.com/rspeer/wordfreq
- **WordNet 3.0** : définitions anglaises et synonymes. © 2006 Princeton University, licence WordNet
  (utilisation, copie et distribution libres, avec cette mention). https://wordnet.princeton.edu

Ce fichier, données dérivées du Wiktionnaire, est partagé sous licence **CC BY-SA 4.0**
(https://creativecommons.org/licenses/by-sa/4.0/). Le code de l'app n'est pas concerné.

Format : une ligne par mot et par nature, champs séparés par une tabulation :
`mot`, `nature` (v, n, adj, adv), `trad1|trad2|trad3`, `définition`, `syn1,syn2`, `exemple avec le [mot] ## traduction || …`.

# Listes de fréquence (`wordlists/`)

Elles servent à choisir les mots de la banque, palier par palier (`scripts/coverage.py`). Les phrases, définitions et
traductions de la banque sont écrites pour LearnToUnlock : seules les listes de mots viennent de ces sources.

- `ngsl-1.01.tsv` : **New General Service List** 1.01, 2 801 mots de l'anglais général, par rang de fréquence.
  Browne, C., Culligan, B. & Phillips, J. (2013). https://www.newgeneralservicelist.com
- `tsl-1.1.tsv` : **TOEIC Service List** 1.1, 1 259 mots propres au TOEIC, par rang. Browne, C. & Culligan, B. (2016).
- `nawl-1.01.tsv` : **New Academic Word List** 1.01, 959 mots de l'anglais universitaire (pour l'après-B2).

Licence des trois listes : **CC BY-SA 4.0**. Fichiers repris du dépôt `antdurrant/word.lists` (données brutes des auteurs).
Les versions 1.2 (2023) déplacent quelques mots d'une liste à l'autre ; à télécharger sur le site des auteurs pour une mise à jour.
