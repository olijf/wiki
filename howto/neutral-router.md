Replacing "massmedia" ISPs routers

Info for Spain / Catalonia

challenge: neutral router that can communicate with GPON technology directly

right now we only can "neutralize" router when it is separated from the ONT

- **movistar**: vlan 6 with generic PPPoE authentication. user: `adslppp@telefonicanetpa` password: adslppp (tested)
- **jazztel**: vlan 1074 with a simple DHCP, sometimes is tricky to get access and you have to wait and/or reboot devices at the same/different time (tested)
- **vodafone**: vlan 100 with custom PPPoE (tested. requires sniffing TR-069 traffic)
    - details step by step, requires separation between router and ont: https://www.redeszone.net/2017/01/21/manual-para-configurar-vodafone-ftth-con-el-sistema-operativo-pfsense-actuando-de-router-neutro/
    - https://bandaancha.eu/articulos/conseguir-admin-router-sercomm-h500-s-9602 but password is VF-ESVodafone-H-500-s

src https://wiki.bandaancha.st/Identificadores_VLAN_operadores_FTTH

src https://naseros.com/2017/02/01/configuracion-de-un-router-neutro-y-configuracion-de-las-vlan/

request: generic procedure for port mirroring
    - (not tested) https://github.com/mmaraya/port-mirroring
    - (not tested) http://www.persianov.net/tutorials/how-to-setup-openwrt-traffic-mirroring-and-snort-ids/
