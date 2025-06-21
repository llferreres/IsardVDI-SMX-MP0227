### Xarxes virtuals

IsardVDI implementa diferents tipus de xarxa. Tot seguit posaré l'equivalència amb VirtualBox

| interficíe VBox | interfície Isard |
|:-----------------:|:------------------:|
| NAT | Default |
| Host-Only | Wireguard VPN |
| Personal1 | Interna |

Existeix un altre tipus de xarxa que vindria a ser com una interna però que permet la connexió pont, és a dir, permet connectar entre altres màquines dintre de l'aula (també a fora, risc de copiar a les proves d'avaluació).  
Aquest altre tipus de xarxa rep el nom de **esteveterradas1**

Si es necessita alguna xarxa d'aquest tipus, es pot demanar la seva creació mitjançant un ticket d'incidència.

### VPN
Per treballar amb VPN, cal descarregar el fitxer de configuració de la VPN i instal·lar el client Wireguard. Veiem com

A la zona superior dreta de la pantalla, on apareix el nom de l'usuari/-a podem fer clic i veure al menú l'opció **VPN**

![19-VPN](https://github.com/user-attachments/assets/8f4472d6-fdbf-425a-92bb-0cf2abefab98)

Per connectar amb la VPN cal instal·lar Wireguard. Ho podem trobar a la web oficial de [Wireguard](https://www.wireguard.com/install/)

Amb Ubuntu podem fer-ne ús així:  
*sudo apt install wireguard*  
*Copiarem el fitxer descarregat de la VPN a la ruta /etc/wireguard*  
*sudo cp isard-vpn.conf /etc/wireguard*

Per utilitzar la connexió:  
*sudo wg-quick up isard-vpn*

Per desconnectar la VPN:  
*sudo wg-quick down isard-vpn*
