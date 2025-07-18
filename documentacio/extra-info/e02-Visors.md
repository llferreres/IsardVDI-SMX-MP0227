### Tipus de visors

Els visors permeten connectar amb la màquina virtual per tal de poder-la utilitzar. Quan crearem escriptoris hem de decidir quin o quins volem que estiguin accessibles. A continuació els comentarem

![18-visors](https://github.com/user-attachments/assets/87b90277-6fd0-40ee-a59c-a12d6bd83b59)

1. El visor **VNC al navegador** es recomana que estigui sempre activat. Tot i se el que menys aporta a facilitar l'ús dels escriptoris, ens permet accedir des d'un navegador web sense necessitat d'instal·lar programari extra, i davant de qualsevol problema de connectivitat és el que sol mantenir accés i ens permetrà treballar. És el més lent, amb pitjor qualitat i el més compatible.

2. **Spice** és el visor recomanat per distribucions GNU/Linux, tot i que també es pot utilitzar amb Microsoft i sistemes Apple. A més de donar millor rendiment a nivell gràfic, també permet la connexió de dispositius USB locals a l'escriptori remot, fins i tot es pot engegar un escriptori Isard des d'un dispositiu local per USB.

*Exemple d'utilització SPICE*

![23-exempleSpice](https://github.com/user-attachments/assets/eb3c0a13-d609-4b1e-a3e3-c133a764948f)

*Per triar USB*

![24-triaUSB](https://github.com/user-attachments/assets/cb8ab98a-adf0-49d7-bffe-1874aef9851e)

*Apareixerà un menú semblant a aquest*

![25-USBs](https://github.com/user-attachments/assets/8c74bb75-e44d-49e6-b8e3-391e16f7c3de)

>[!WARNING]
>Utilitzar l'opció d'afegir un dispositiu local a IsardVDI el desactivarà del dispositiu local, el que podria repercutir en perdre el teclat, la webcam o accés a carpetes si les necessitem en local.

Per descarregar el programari d'instal·lació, podeu accedir a aquest [enllaç](https://www.spice-space.org/download.html)  
Per Ubuntu: *sudo apt install virt-viewer*

4. **RDP** és el protocol d'escriptori remot de Microsoft, per tant s'adequa millor per utilitzar-ho amb sistemes Microsoft Windows. Tenim una versió per obrir des d'un navegador, una versió per utilitzar el client RDP i una darrera versió per utilitzar amb la [VPN](https://github.com/llferreres/IsardVDI-SMX-MP0227/blob/main/documentacio/extra-info/e01-xarxes.md#vpn) que proporciona Isard.
