French customers. Enedis has recently introduced production mode (letter P on the Linky) for some of their photovoltaic producer customers who do not have a sales contract because their injection into the public network is too high.
These customers become liable for the TURPE.
With the aim of reducing this unwanted injection, I've looked into how to avoid it with simple automations that are easy to set up for the uninitiated, whether French or not.

Clients Français. Depuis peu Enedis a mis en place le mode production (lettre P apparaissant sur le Linky) chez certains de leurs clients producteur photovoltaïque alors qu'ils n'ont pas de contrat de vente car leur injection sur le réseau public est trop élevé.
Ceux ci deviennent redevable de la TURPE.
Dans le but de réduire cette injection non désirée, j'ai cherché comment l'éviter avec de simples automations simple à mettre en place pour les non initiés, français ou pas, le plus compliqué étant de récupérer les sensors dans les différentes intégrations.


Vous avez le choix entre:
- le limiteur auto micro onduleur Deye (le sensor arrive par l'intégration Solarman)
- le limiteur auto HMS Hoyamiles (le sensor arrive en MQTT via Opend DTU)
- le limiteur auto mixant avec des priorités modifiables entre le Deye et le Hoymiles
- le limiteur auto mixant Deye + HMS avec ondition de la charge batteries Zendure (hyper ou autres batteries) (intégration Fireson)
- le limiteur auto Deye+HMS+ Bat avec selecteur de mode et son board.
