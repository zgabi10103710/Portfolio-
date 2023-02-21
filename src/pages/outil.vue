<template>
  <div class="container">


      <BinaryTextSVG />
      <h1 class="about-content__headline">Outils</h1>

    <main id="main-content">
      <article class="about-content">


      <p>
      <ul>
      <br>

        <li> Impacket ( <a href=" https://github.com/SecureAuthCorp/impacket"> Impacket </a> )
        Une suite d'outils développés en Python pour interagir avec les différents protocoles réseau
        </li>
        <br>

        <li>
        - Mimikatz ( <a href=" https://blog.gentilkiwi.com/mimikatz">mimikatz</a>)
        Outil développé en C qui permet de voir et enregistrer des informations d’authentification comme des tickets Kerberos
</li>
<br>

<li>
        - Pypykatz (<a href="  https://github.com/skelsec/pypykatz">pypykatz</a>)
        Une réécriture de Mimikatz entièrement en Python
</li>
<br>

<li>
        - Rubeus ( <a href=" https://github.com/GhostPack/Rubeus">Rubeus</a>)
        Ensemble de fonctions développées en C# pour interagir et les abuser du protocole Kerberos
</li>
<br>
<li>

        - CrackMapExec (<a href="  https://github.com/Porchetta-Industries/CrackMapExec">CrackMapExec</a>)
        Outil de post-exploitation qui permet d'automatiser l'évaluation de la sécurité d'Active Directory
        </li>
        <br>
        <li>

        - NetCat (<a href="  https://fr.wikipedia.org/wiki/Netcat">NetCat</a>)
        Outil en ligne de commande permettant d'écrire et de lire des données au niveau du réseau
        </li>
        <br>
        <li>

        - PowerSploit (<a href="  https://github.com/PowerShellMafia/PowerSploit">PowerSploit</a>)
        Collection de modules PowerShell pouvant être utilisés pour aider les pentesters pendant toutes les phases d'une évaluation
        </li>
        <br>
        <li>

        - BloodHound ( <a href=" https://github.com/BloodHoundAD/BloodHound">BloodHound</a>)
        Application Web qui utilise la théorie des graphes pour révéler les relations cachées et souvent involontaires au sein d'un environnement Active Directory ou Azure
        </li>
        <br>
        <li>

        - Responder ( <a href=" https://github.com/SpiderLabs/Responder">Responder</a>)
        Empoisonneur LLMNR, NBT-NS et MDNS, avec serveur d'authentification HTTP/SMB/MSSQL/FTP/LDAP intégré prenant notamment en charge NTLM

        </li>
        <br>
        <li>
        - PetitPotam (<a href="  https://github.com/topotam/PetitPotam">PetitPotam</a>)
        Outil PoC pour contraindre les hôtes Windows à s'authentifier auprès d'autres machines via MS-EFSRPC EfsRpcOpenFileRaw ou d'autres fonctions
        </li>
        <br>
        <li>

        - Coercer (<a href="  https://github.com/p0dalirius/Coercer">Coercer</a>)
        Script python pour contraindre automatiquement un serveur Windows à s'authentifier sur une machine arbitraire via plusieurs méthodes

        </li>
        <br>
        <li>
        - Certipy ( <a href=" https://github.com/ly4k/Certipy">Certipy</a>)
        Outil offensif pour énumérer et abuser des services de certificats Active Directory (AD CS)
        </li>
        <br>
        <li>

        - Evil-WinRM ( <a href=" https://github.com/Hackplayers/evil-winrm">evil</a>)
        Réimplémentation de Microsoft WinRM (Windows Remote Management) et du protocole de gestion WS développé en Ruby

        </li>
        <br>
        <li>
        - DonPAPI ( <a href=" https://github.com/login-securite/DonPAPI">DonPAPI</a>)
        Outil permettant de récupérer à distance les secrets DPAPI d'un poste
        </li>
        <br>
        <li>

        - Hekatomb ( <a href=" https://github.com/Processus-Thief/HEKATOMB">HEKATOMB</a>)
        Outil de post-exploitation de test d'intrusion permettant de récupérer et déchiffrer les identifiants DPAPI des postes d'un domaine Active Directory

        </li>
        <br>
        <li>
        - Nmap (<a href=" https://nmap.org">NMAP</a>)
        Probablement le scanneur de réseau le plus complet
        </li>
        <br>
        <li>

        - Nikto (<a href="  https://github.com/sullo/nikto">nikto</a>)
        Scanner de vulnérabilités web
        </li>
        <br>
        <li>

        - Burp Suite ( <a href=" https://portswigger.net/burp">burp suite</a>)
        Outil permettant de proxifier des requêtes web afin de pouvoir les modifier et les rejouer
        </li>
        <br>
        <li>

        - Gobuster ( <a href=" https://github.com/OJ/gobuster">gobuster</a>)
        Outil de fuzzing (bruteforce) d'URL et de sous-domaines DNS développé en Go
        </li>
        <br>
        <li>

        - SQLMap ( <a href=" https://github.com/sqlmapproject/sqlmap">SQLMAP</a>)
        Outil de test d'intrusion open source qui automatise le processus de détection et d'exploitation d'injections SQL
        </li>
        <br>
        <li>

        - John The Ripper (<a href="  https://www.openwall.com/john">john</a>)
        Outil Open Source d'audit de sécurité et de bruteforce de mots de passe

        </li>
        <br>
        <li>
        - Hashcat ( <a href=" https://github.com/hashcat/hashcat">Hashcat</a>)
        Outil de bruteforce de mots de passe supportant l'utilisation de périphériques graphiques

        </li>
        <br>
        <li>
        - Aircrack-Ng ( <a href=" https://github.com/aircrack-ng/aircrack-ng">Aircrack</a>)
        Outil Open Source d'audit de sécurité WIFI
        </li>
        <br>
        <li>

        - Ettercap ( <a href=" https://github.com/Ettercap/ettercap">Ettercap</a>)
        Outil d'empoisonnement de requêtes ARP permettant d'effectuer une attaque de type Man In The Middle

        </li>
        <br>
        <li>
        - Metasploit (<a href=" https://www.metasploit.com">MetaSploit</a>)
        Suite d'outils développés par Rapid7 en Ruby permettant de contrôler des cibles distantes (serveur C2)
        </li>
        <br>
        <li>

        - Cobalt Strike (<a href=" https://www.cobaltstrike.com">cobaltstrike</a>)
        Suite d'outils permettant de contrôler des cibles distantes (serveur C2) auparavant basé sur MetaSploit
        </li>
        <br>
        <li>

        - Arsenal ( <a href=" https://github.com/Orange-Cyberdefense/arsenal">Arsenal</a>)
        Suite d'outils permettant de contrôler des cibles distantes (serveur C2) développé en Python par Orange Cyberdefense
        </li>
        <br>
        <li>

        - Volatility ( <a href=" https://github.com/volatilityfoundation/volatility">volatility</a>)
        Outil d'investigation avancée de mémoire volatile (RAM) et de partitions de disque
        </li>
        <br>
        <li>

        - Wireshark ( <a href=" https://www.wireshark.org/download.html">wireshark</a>)
        Outil d'analyse de protocoles réseau
        </li>
        <br>
        <li>

        - YARA ( <a href=" https://www.kali.org/tools/yara">YARA</a>)
        Outil destiné à aider les chercheurs en sécurité à identifier et classer les échantillons de logiciels malveillants

        </li>
        <br>
        <li>
        - Caldera ( <a href=" https://github.com/mitre/caldera">Caldera</a>)
        Plate-forme automatisée d'émulation d'attaques informatiques principalement déveoppée en Python
        </li>
        <br>
        <li>

        - Atomic Red Team ( <a href=" https://github.com/redcanaryco/atomic-red-team">Atomic Red Team</a>)
        Plate-forme automatisée d'émulation d'attaques informatiques basées sur le MITRE ATT&CK
        </li>
        <br>
        <li>

        - The Hive (<a href=" https://thehive-project.org">The Hive</a>)
        Console de réponse à incidents de sécurité
        </li>
        <br>
        <li>

        - MISP (<a href=" https://www.misp-project.org ">MISP</a>)
        Plate-forme open source de renseignement et de partage des menaces
</li>
      </ul>
      </p>






      </article>
    </main>
  </div>
</template>

<script setup>
import { useRoute } from 'vue-router'
import config from '../config/siteconfig.json'

const title = 'About me • Gabriel Briziou '
const { description } = config
const route = useRoute()

useHead({
  title,
  meta: [
    {
      name: 'description',
      content: description,
    },
    { property: 'og:type', content: 'website' },
    { property: 'og:title', content: title },
    { property: 'og:description', content: description },
    { property: 'og:url', content: `${config.siteUrl}${route.path}` },
    {
      property: 'twitter:title',
      content: title,
    },
    {
      property: 'twitter:description',
      content: description,
    },
  ],
})
</script>

<route lang="yaml">
meta:
  layout: default
</route>

<style lang="css" scoped>
:global(#app) {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.container {
  flex-flow: row wrap;
  padding: 3rem 0;
}

main {
  padding: 1.2rem 2.4rem;
}

.about-content {
  .about-content__headline {
    font-size: var(--text-2xl);
  }

  p {
    font-size: var(--text-lg);
    opacity: 0.8;
    max-width: 71ch;
  }
}

.binary-text-svg {
  font-family: var(--font-mono);
  font-size: var(--text-xl);
  position: absolute;
  left: 282px;
  top: 387px;
  opacity: 0.3;

  & :deep(tspan) {
    --text-delay: 500ms;

    opacity: 0;
    animation: pulse-spread 3s var(--text-delay) ease-out infinite alternate;

    &:nth-child(1) {
      --text-delay: 500ms;
    }

    &:nth-child(2) {
      --text-delay: 1s;
    }

    &:nth-child(3) {
      --text-delay: 1.5s;
    }

    &:nth-child(4) {
      --text-delay: 2s;
    }

    &:nth-child(5) {
      --text-delay: 2.5s;
    }

    &:nth-child(6) {
      --text-delay: 3s;
    }
  }
}

@keyframes pulse-spread {
  0% {
    opacity: 0;
  }

  100% {
    opacity: 0.3;
  }
}

@media screen and (min-width: 426px) and (max-width: 768px) {
  aside {
    margin-left: 40px;
    padding: 0 2.4rem 0 0;
  }
}

@media screen and (max-width: 425px) {
  aside {
    padding: 0 1rem;
  }

  .container {
    height: 100%;
  }

  .binary-text-svg {
    top: 50%;
    left: 0;
    bottom: 0;
  }
}
</style>
