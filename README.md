# TP3_ZacharyGagnon

## Description:
ce projet a pur but de demontre mes apprentissage au niveau de la comprehension des proxy, des serveur relier a celui-ci ainsi que la relation entre eux 

## Explication:
lorsque que l'ont veut demmare le serveur nous utilison docker compose
```
docker compose up -d
```
ce qui vas creer plusieur containeur:
- un proxy nginx
- deux serveur apache (httpd) distinc
- deux php (pour chaque apache)
- deux maraidb (pour chaque apache)
pour pouvoir voire si les containeur roule bien utliser la commande:
```
docker compose ps
```
et pour verifier les log utiliser:
```
docker compose logs
```
et pour voire les log de connexion au proxy utiliser:
```
docker compose logs proxy
```
donc lorsque tout les container sont creer le proxy vas appaler les deux serveur apache qui vont a leur tour appeler leur serveur php et maraidb respectif.
pour finir arreter les container avec cette commade:
```
docker compose down --rmi local -v
```
qui permet aussi de enlever les image et volume utiliser 
