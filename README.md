
**Adresses IP : **

**octet 1 . octet 2 . octet 3 . octet 4**

**1 octet = 8 bits**

XXXX XXXX . XXXX XXXX . XXXX XXXX . XXXX XXXX

**Exemple:**

10000000.00001010.11011000.00100111

=

128.10.216.39


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
   <td><strong>Partie Réseaux</strong>
<p>
<strong>Partie Hotes</strong>
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
   <td>0XXX XXXX
   </td>
   <td>XXXX XXXX
   </td>
   <td>XXXX XXXX
   </td>
   <td>XXXX XXXX
   </td>
  </tr>
  <tr>
   <td>Classe B
   </td>
   <td>XXXX XXXX
   </td>
   <td>XXXX XXXX
   </td>
   <td>XXXX XXXX
   </td>
   <td>XXXX XXXX
   </td>
  </tr>
  <tr>
   <td>Classe C
   </td>
   <td>110X XXXX
   </td>
   <td>XXXX XXXX
   </td>
   <td>XXXX XXXX
   </td>
   <td>XXXX XXXX
   </td>
  </tr>
</table>


**Combien d'hôtes et de sous réseaux peut-il y avoir avec le masque suivant ? **

**255.255.255.240**

240.0 = **1111 0000** . **0000 0000**

**12 bits pour les hôtes : **

2^12 = 4096 => - 2 ( - ip de réseau - ip de diffusion) => **4094 hôtes**

**4 bits pour les sous réseaux :**

2^4 = 16 sous réseaux.

**Un reseau a comme adresse 180.35.128.0 de masque 255.255.240.0. Quelle est l’adresse de diffusion ou broadcast ?**

180.35.128.0 est une adresse de classe B. Ce sont donc les deux derniers octets qui définissent la partie hôte.

240.0 = 1111 0000 . 0000 0000

128.0 = 1000 0000 . 0000 0000

1111 0000 . 0000 0000

1000 0000 . 0000 0000

= 

1000 1111 . 1111 1111 = 143.255

**Adresse de diffusion finale = 180.35.143.255**

**Créer 3 sous réseaux sur le réseau suivant : **

192.168.4.0/24


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


On choisit la colonne aux 4 sous réseaux :

**On a donc 64 hôtes possibles par sous réseaux.**


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
