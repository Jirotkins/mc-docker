# Minecraft server v Dockeru
Tento projekt je založen na Dockeru a umožňuje snadnou implementaci a správu Minecraft serveru s modifikacemi z CurseForge. Kromě toho používám nástroje jako Prometheus pro sběr dat ze serveru
 a Grafana pro jejich vizualizaci. Server je zde už sestavený a připravený jen na spuštění.

## Návod na spuštění
1. ``` git clone https://github.com/jirotkins/mc-docker ```
2. přejděte do adresáře projektu ``` cd mc-docker ```
3. ``` docker compose up -d ```

* Server se chvíli bude pouštět, pak se můžeme podívat na sběr dat na Grafaně. ``` localhost:3000 ```
* Prometheus běží na portu ``` 9090 ```
* Minecraft server na ``` 25565 ``` 
* V případě změny modpacku stačí v ``` docker-compose.yml ``` změnit URL na modpack nebo nastavit typ serveru na vanillu a mody odstranit.
