# synology-diskstation-zabbix-snmpv3
Synology Diskstation Template for Zabbix supporting SNMPv3  
Based on https://share.zabbix.com/storage-devices/synology/synology-diskstation  
  
DiskStationManager > Terminal SNMP > SNMP > Enable SNMPv3   
Enable SNMP service
    enable SNMPv3 service
    Username: $username
    Protocol: SHA
    Password: $authpassword
    Enable SNMP privacy
        Protocol: AES
        Password: $privpassword

Zabbix
6.0
SNMP version: SNMPv3
Security name: $username
Security level: authPriv
Authentication protocol: SHA1
Authentication passphrase: $authpasswort 
Privacy protocol: AES128
Privacy passphrase: $privpasswort