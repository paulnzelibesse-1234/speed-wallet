<h1 align="center"><strong>🚀 PROCESS DE DEPLOIEMENT D'UNE APPLICATION</strong></h1><br>
<p>
Pour déployer votre application, vous avez plusieurs techniques et outils possible selon votre type d'application et votre catégorie de serveur (serveur mutualisé, serveur dédié ...) et vos besoins.
NB :
</p><br>
<h2 align="center"><strong>💡 Types de serveurs</strong></h2>

<p><strong>🔹 Serveur mutualisé</strong><br>
Si vous utilisez un <strong>serveur mutualisé</strong> (achat d'une partie de l'espace d'hébergement auprès d’un fournisseur de services), <strong>aucune configuration particulière n'est généralement requise</strong>, car le fournisseur se charge de l'installation et du partage des ressources entre les différents utilisateurs.</p>

<p><strong>🔹 Serveur dédié</strong><br>
En revanche, si vous utilisez un <strong>serveur dédié</strong>, le serveur vous appartient entièrement. Vous êtes donc responsable de l’ensemble des <strong>configurations nécessaires</strong> au bon fonctionnement de vos applications.</p>

<hr>

<h2 align="center"><strong>🚀 Cas pratique : Déploiement d'une application Java/Spring 🌱 et Angular 🚀 sur un serveur dédié (Oracle Linux)</strong></h2>

<h3><strong>🔰 Par où commencer ?</strong></h3>

<p>Commencez par installer les outils nécessaires sur votre serveur.<br>
Dans notre cas particulier, les éléments suivants seront requis :</p>

<ul>
  <li>✅ Vérifier la version du système Oracle Linux</li>
  <li>✅ Installer un <strong>JDK</strong> (choisir la <strong>même version</strong> que celle utilisée pour développer l'application)</li>
  <li>✅ Installer une version de <strong>PHP</strong> (si nécessaire selon votre environnement)</li>
  <li>✅ Installer et configurer un <strong>serveur Nginx</strong> (nous l’utiliserons dans ce guide) ou <strong>Apache</strong> en alternative</li>
</ul>

<h3><strong>📦 Note importante – Gestionnaire de paquets</strong></h3>

<p>Sur Oracle Linux, deux gestionnaires de paquets principaux sont utilisés en fonction de la version du système :</p>

<ul>
  <li><code>yum</code> → pour Oracle Linux <strong>7</strong></li>
  <li><code>dnf</code> → pour Oracle Linux <strong>8 et versions supérieures</strong></li>
</ul>

<h4><strong>🔍 Vérifier la version de votre serveur :</strong></h4>

<pre>
<code>cat /etc/os-release</code>
</pre
  
<h2 align="center"><strong>🖼️ Un aperçu en image</strong></h2>
<p align="center">
  <img src="/assets/images/cap1.png" alt="Aperçu" width="600">
</p>
<p>Nous utilisons un <strong>serveur Oracle Linux 8</strong>, ce qui signifie que les commandes que nous allons utiliser commenceront par <code>dnf</code>.</p>


