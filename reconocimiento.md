# NMAP
**Escaneamos los puertos abiertos con NMAP**

nmap -p- --open -T5 -v IP_VICTIMA
nmap -p- -sS --min-rate 5000 --open -vvv -n IP_VICTIMA  -Pn -oG puertos.txt

**Enumeramos las versiones y servicios de los puertos abiertos**

nmap -sCV -pPuerto1,Puerto2 IP_VICTIMA -oN AnalisisPuertos.txt