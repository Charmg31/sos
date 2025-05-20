French customers. Enedis has recently introduced production mode (letter P on the Linky) for some of their photovoltaic producer customers who do not have a sales contract because their injection into the public network is too high.
These customers become liable for the TURPE.

In order to reduce this unwanted injection, I looked into how to avoid it with simple automations that are easy to set up for the uninitiated, whether French or not. The most complicated part is retrieving the sensors from the various integrations.
Because of their design, some microinverters like Deye don't like strong power variations, especially at full load, nor too rapid changes. You need to take this into consideration in your automation, and the one I propose here is progressive, acting in steps, so don't overstress the microinverters: the optimum timing is 15 seconds.


You can choose between:

the Deye microinverter auto limiter (the sensor arrives via Solarman integration)
the Hoyamiles HMS auto limiter (the sensor arrives in MQTT via Opend DTU)
the mixing auto limiter with modifiable priorities between the Deye and the Hoymiles
the Deye + HMS mixing auto limiter with Zendure battery charge condition (hyper or other batteries) (Fireson integration)
the Deye+HMS+ Bat auto limiter with mode selector and its board.




Clients Français. Depuis peu Enedis a mis en place le mode production (lettre P apparaissant sur le Linky) chez certains de leurs clients producteur photovoltaïque alors qu'ils n'ont pas de contrat de vente car leur injection sur le réseau public est trop élevé.
Ceux ci deviennent redevable de la TURPE.
Dans le but de réduire cette injection non désirée, j'ai cherché comment l'éviter avec de simples automations simple à mettre en place pour les non initiés, français ou pas, le plus compliqué étant de récupérer les sensors dans les différentes intégrations.
De part leur conception certains micro onduleurs comme les Deye n'aiment pas trop à terme les fortes variations de puissance surtout en pleine charge ni les changements trop rapides, il faut en tenir compte dans les automatisations, celle que je propose ici sont progressives, elles agissent par pallier, pensez aussi à ne pas trop stresser les micro onduleurs, le timing optimum est de 15 secondes. 


Vous avez le choix entre:
- le limiteur auto micro onduleur Deye (le sensor arrive par l'intégration Solarman)
- le limiteur auto HMS Hoyamiles (le sensor arrive en MQTT via Opend DTU)
- le limiteur auto mixant avec des priorités modifiables entre le Deye et le Hoymiles
- le limiteur auto mixant Deye + HMS avec condition de la charge batteries Zendure (hyper ou autres batteries) (intégration Fireson)
- le limiteur auto Deye+HMS+ Bat avec selecteur de mode et son board.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Dernier en date et le plus abouti, [Deye_HMS_No_Inject_PID](https://github.com/Charmg31/sos#:~:text=last%20week-,Deye_HMS_No_Inject_PID,-Create%20Deye_HMS_No_Inject_PID)
Comment l'utiliser?
1. Ajoutez ce [bloc ](https://github.com/Charmg31/sos/blob/main/Input_select_configuration_%20yaml)dans votre fichier configuration.yaml :


2.  Méthode rapide (YAML brut)
Aller dans Paramètres → Automatisations et scènes → Automatisations.

Cliquez sur Ajouter une automatisation puis sur Démarrer avec une automatisation vide.

En haut à droite, cliquez sur ⋮ (trois points) puis Modifier en YAML.

Collez votre code YAML dans l’éditeur.

Personalisez/adaptez à votre propre sensor de sonde

Cliquez sur Enregistrer.
3. Option dashboard 
[Deye+HMS+YK](https://github.com/Charmg31/sos/blob/main/Deye%2BHMS%2BYK%20selector%20dashboard) selector dashboard est un dash bord à modifier suivant vos besoins


