<p>
<strong>Adresses IP</strong>
</p>
<p>
<strong>octet 1 . octet 2 . octet 3 . octet 4</strong>
</p>
<p>
<strong>1 octet = 8 bits</strong>
</p>
<p>
XXXX XXXX . XXXX XXXX . XXXX XXXX . XXXX XXXX
</p>
<p>
<strong>Exemple:</strong>
</p>
<p>
10000000.00001010.11011000.00100111 = 128.10.216.39
</p>

<table>
  <tr>
   <td>Classe A
   </td>
   <td>0
   </td>
   <td>0.0.0.0
   </td>
   <td>127.255.255.255
   </td>
  </tr>
  <tr>
   <td>Classe B
   </td>
   <td>10
   </td>
   <td>128.0.0.0
   </td>
   <td>191.255.255.255
   </td>
  </tr>
  <tr>
   <td>Classe C
   </td>
   <td>110
   </td>
   <td>192.0.0.0
   </td>
   <td>223.255.255.255
   </td>
  </tr>
  <tr>
   <td>Classe D
   </td>
   <td>1110
   </td>
   <td>224.0.0.0
   </td>
   <td>239.255.255.255
   </td>
  </tr>
</table>



<table>
  <tr>
   <td>
   </td>
   <td>Octet 1
   </td>
   <td>Octet 2
   </td>
   <td>Octet 3
   </td>
   <td>Octet 4
   </td>
  </tr>
  <tr>
   <td>Classe A
   </td>
   <td>Réseau
   </td>
   <td>Hôtes
   </td>
   <td>Hôtes
   </td>
   <td>Hôtes
   </td>
  </tr>
  <tr>
   <td>Classe B
   </td>
   <td>Réseau
   </td>
   <td>Réseau
   </td>
   <td>Hôtes
   </td>
   <td>Hôtes
   </td>
  </tr>
  <tr>
   <td>Classe C
   </td>
   <td>Réseau
   </td>
   <td>Réseau
   </td>
   <td>Réseau
   </td>
   <td>Hôtes
   </td>
  </tr>
</table>


<table>
  <tr>
   <td colspan="4" ><strong>Masques de sous réseaux</strong>
   </td>
  </tr>
  <tr>
   <td><strong>Classiques</strong>
   </td>
   <td><strong>CIDR</strong>
   </td>
   <td><strong>Hôtes</strong>
   </td>
   <td><strong>Sous Réseaux</strong>
   </td>
  </tr>
  <tr>
   <td>255.255.255.0
   </td>
   <td>/24
   </td>
   <td>256
   </td>
   <td>1
   </td>
  </tr>
  <tr>
   <td>255.255.255.128
   </td>
   <td>/25
   </td>
   <td>128
   </td>
   <td>2
   </td>
  </tr>
  <tr>
   <td>255.255.255.192
   </td>
   <td>/26
   </td>
   <td>64
   </td>
   <td>4
   </td>
  </tr>
  <tr>
   <td>255.255.255.224
   </td>
   <td>/27
   </td>
   <td>32
   </td>
   <td>8
   </td>
  </tr>
  <tr>
   <td>255.255.255.240
   </td>
   <td>/28
   </td>
   <td>16
   </td>
   <td>16
   </td>
  </tr>
  <tr>
   <td>255.255.255.248
   </td>
   <td>/29
   </td>
   <td>8
   </td>
   <td>32
   </td>
  </tr>
  <tr>
   <td>255.255.255.252
   </td>
   <td>/30
   </td>
   <td>4
   </td>
   <td>64
   </td>
  </tr>
  <tr>
   <td>255.255.255.254
   </td>
   <td>/31
   </td>
   <td>2
   </td>
   <td>128
   </td>
  </tr>
  <tr>
   <td>255.255.255.255
   </td>
   <td>/32
   </td>
   <td>1
   </td>
   <td>256
   </td>
  </tr>
</table>


</br>
</br>
</br>
</br>
<p>
<strong>Exercice 1 :</strong>
</p>
<p>
<strong>Combien d'hôtes et de sous réseaux peut-il y avoir avec le masque suivant ? </strong>
</p>
<p>
<strong>255.255.255.240</strong>
</p>
<p>
240.0 = <strong>1111 0000</strong> . <strong>0000 0000</strong>
</p>
<p>
<strong>12 bits pour les hôtes : </strong>
</p>
<p>
2^12 = 4096 => - 2 ( - ip de réseau - ip de diffusion) => <strong>4094 hôtes</strong>
</p>
<p>
<strong>4 bits pour les sous réseaux :</strong>
</p>
<p>
2^4 = 16 sous réseaux.
</p>
<p>
</br>
</br>
</br>
</br>
<strong>Exercice 2 :</strong>
</p>
<p>
<strong>Un reseau a comme adresse 180.35.128.0 de masque 255.255.240.0. Quelle est l’adresse de diffusion ou broadcast ?</strong>
</p>
<p>
180.35.128.0 est une adresse de classe B. Ce sont donc les deux derniers octets qui définissent la partie hôte.
</p>
<p>
240.0 = 1111 0000 . 0000 0000
</p>
<p>
128.0 = 1000 0000 . 0000 0000
</p>
<p>
1111 0000 . 0000 0000
</p>
<p>
1000 0000 . 0000 0000
</p>
<p>
= 
</p>
<p>
1000 1111 . 1111 1111 = 143.255
</p>
<p>
<strong>Adresse de diffusion finale = 180.35.143.255</strong>
</p>
<p>
</br>
</br>
</br>
</br>
<strong>Exercice 3 :</strong>
</p>
<p>
<strong>Créer 3 sous réseaux sur le réseau suivant : </strong>
</p>
<p>
192.168.4.0/24
</p>

<table>
  <tr>
   <td>Sous réseaux
   </td>
   <td>1
   </td>
   <td>2
   </td>
   <td>4
   </td>
   <td>8
   </td>
   <td>16
   </td>
   <td>32
   </td>
   <td>64
   </td>
   <td>128
   </td>
   <td>256
   </td>
  </tr>
  <tr>
   <td>Hôte
   </td>
   <td>256
   </td>
   <td>128
   </td>
   <td>64
   </td>
   <td>32
   </td>
   <td>16
   </td>
   <td>8
   </td>
   <td>4
   </td>
   <td>2
   </td>
   <td>1
   </td>
  </tr>
  <tr>
   <td>Masque de sr
   </td>
   <td>/24
   </td>
   <td>/25
   </td>
   <td>/26
   </td>
   <td>/27
   </td>
   <td>/28
   </td>
   <td>/29
   </td>
   <td>/30
   </td>
   <td>/31
   </td>
   <td>/32
   </td>
  </tr>
</table>


<p>
On choisit la colonne aux 4 sous réseaux :
</p>
<p>
<strong>On a donc 64 hôtes possibles par sous réseaux.</strong>
</p>

<table>
  <tr>
   <td><strong>ID réseau</strong>
   </td>
   <td><strong>Masque</strong>
   </td>
   <td><strong>Plage d’ip hôte</strong>
   </td>
   <td><strong>Nombre d'hôte</strong>
   </td>
   <td><strong>@ Broadcast</strong>
   </td>
  </tr>
  <tr>
   <td>192.168.4.<strong>0</strong>
   </td>
   <td>/26
   </td>
   <td>1 - 62
   </td>
   <td>62 (64 - 2)
   </td>
   <td>192.168.4.<strong>63</strong>
   </td>
  </tr>
  <tr>
   <td>192.168.4<strong>.64</strong>
   </td>
   <td>/26
   </td>
   <td>65 - 126
   </td>
   <td>62 (64 - 2)
   </td>
   <td>192.168.4.<strong>127</strong>
   </td>
  </tr>
  <tr>
   <td>192.168.4.<strong>128</strong>
   </td>
   <td>/26
   </td>
   <td>129 - 190
   </td>
   <td>62 (64 - 2)
   </td>
   <td>192.168.4.<strong>191</strong>
   </td>
  </tr>
  <tr>
   <td>192.168.4.<strong>192</strong>
   </td>
   <td>/26
   </td>
   <td>192 - 254
   </td>
   <td>62 (64 - 2)
   </td>
   <td>192.168.4.<strong>255</strong>
   </td>
  </tr>
</table>
