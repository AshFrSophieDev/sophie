Principe du jeu
Les spectateurs (viewers) doivent s'occuper d'une patiente virtuelle via des commandes dans le chat Twitch afin de la maintenir en vie et en bonne santé :

Constantes suivies : Points de vie (hp), hydratation (hydro), température (temp), ainsi que différents états médicaux (éruption cutanée, anasarque / surcharge hydrique, étouffement, intubation, sédation, arrêt cardiaque).
Évolution automatique (gameTick) : Toutes les 15 secondes, la patiente perd progressivement de l'hydratation et des points de vie, peut développer une éruption cutanée aléatoire, ou faire un arrêt cardiaque si elle s'étouffe ou tombe à 0 PV.
Commandes du chat :
Nourrir : !manger, !sandwich, !cacahuetes (redonne des PV, avec un risque de fausse route / étouffement).
Hydratation : !eau / !perfusion (+20 % d'hydratation, attention à l'anasarque au-dessus de 150 %) et !lasilix / !diuretique (-20 %).
Soins courants : !doliprane (baisse la température), !creme / !antihistaminique (soigne l'éruption).
Urgences & Réanimation : !heimlich (en cas d'étouffement), !intuber, !sedater (!hypnovel), !reveiller, !extuber, et !mace / !cpr / !massage (en cas d'arrêt cardiaque).
État actuel des fichiers
index.js : Contient toute la logique du jeu, la gestion des événements StreamElements (onEventReceived) et la mise à jour de l'interface.
index.html et index.css : Ces deux fichiers sont actuellement vides (0 ligne). Il manque donc la structure HTML et le style CSS associés aux identifiants utilisés dans le script (#patient-img, #patient-status, #hp-bar, #hydro-bar, #temp-bar, #log-box, etc.).