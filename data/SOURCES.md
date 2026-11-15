# Dictionnaire anglais → français de LearnToUnlock

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
