# Epicode – Consegne

Raccolta dei report delle esercitazioni svolte durante il corso di cybersecurity di Epicode.
Ogni PDF è il report di una lezione, nominato nel formato `SxLy` (Settimana *x*, Lezione *y*),
e documenta un'attività pratica svolta in un ambiente di laboratorio isolato (macchine virtuali
e Cisco Packet Tracer).

## Settimana 1 – Fondamenti di rete

- **S01L1** – Report di verifica del setup del laboratorio: controllo del corretto funzionamento delle macchine virtuali Windows 7, Kali Linux e Metasploitable.
- **S01L2** – Esercizi di subnetting: per una serie di indirizzi IP con notazione CIDR si calcolano maschera di sottorete, indirizzo di rete, primo e ultimo host e indirizzo di broadcast.
- **S01L3** – Realizzazione in Packet Tracer di una rete con due switch e sei host (tre per switch) tutti nella stessa rete (192.168.88.1–6), con verifica della comunicazione tramite ping.
- **S01L4** – Rete a due sottoreti collegate da un router in Packet Tracer, usata per spiegare le comunicazioni ai livelli 2 (ARP e indirizzi MAC) e 3 (IP, gateway, routing) del modello ISO/OSI.
- **S01L5** – Progettazione di una rete segmentata in quattro VLAN, con spiegazione delle differenze tra VLAN e subnetting e delle motivazioni della scelta.

## Settimana 2 – Programmazione in C e Python

- **S02L1** – Configurazione di un server DHCP in Packet Tracer per assegnare dinamicamente gli IP di un range, con router, switch e server.
- **S02L2** – Due programmi in C: moltiplicazione di due numeri inseriti dall'utente e calcolo della media aritmetica; documenta anche l'uso del terminale (mkdir, nano, compilazione).
- **S02L3** – Script Python che genera un "nome da band" combinando città e nome di un animale, con validazione dell'input per gestire i valori vuoti.
- **S02L4** – Programma Python a menu per calcolare il perimetro di diverse figure geometriche (quadrato, cerchio, rettangolo) con error handling e uso del modulo `math`.
- **S02L5** – Analisi statica di un codice sorgente: capire cosa fa senza eseguirlo, individuare i casi non gestiti e gli errori logici/sintattici e proporre una soluzione per ciascuno.

## Settimana 3 – Scheduling, web security e crittografia

- **S03L1** – Studio dello scheduling della CPU su quattro processi con tempi di esecuzione e attesa I/O dati: scelta del metodo più efficace e diagramma temporale dell'esecuzione.
- **S03L2** – Esercizio di programmazione (il report è contrassegnato dall'autore come work in progress).
- **S03L3** – Installazione e configurazione di DVWA su Kali (MySQL e Apache) e intercettazione/modifica della richiesta di login con Burp Suite, mostrando la password in chiaro su HTTP.
- **S03L4** – Decodifica di una stringa cifrata: riconoscimento della codifica Base64 e dei cifrari ROT, con uno script Python che applica lo shift delle lettere.
- **S03L5** – Installazione di pfSense come firewall per filtrare il traffico tra Kali e Metasploitable/DVWA, poste su due reti diverse.

## Settimana 5 – Scanning e vulnerability assessment

- **S05L2** – OS detection e port scanning con nmap su più sistemi (Metasploitable, Windows 10), confrontando gli switch `-O`, `--osscan-guess` e lo script `smb-os-discovery`.
- **S05L3** – Vulnerability scanning di Metasploitable con Nessus sulle porte comuni, con analisi del report e delle vulnerabilità note rilevate.
- **S05L5** – Creazione di una simulazione di email di phishing (scenario di notifica bancaria) a scopo di studio, con analisi degli elementi che la rendono credibile e di quelli sospetti; include una versione HTML.

## Settimana 6 – Exploitation e brute forcing

- **S06L2** – Sfruttamento, a scopo didattico su DVWA con sicurezza LOW, di una vulnerabilità XSS reflected e di una SQL injection non blind.
- **S06L3** – Script Python di UDP flooding (moduli `socket` e `random`) verso IP e porta scelti, con numero di pacchetti configurabile.
- **S06L5** – Cracking dell'autenticazione di servizi di rete (SSH e FTP) con Hydra e le wordlist di SecLists, su un utente di test creato appositamente.

## Settimana 7 – Metasploit e anonimato

- **S07L1** – Exploit del servizio vsftpd di Metasploitable con Metasploit e uso della shell remota per creare una cartella nella directory root.
- **S07L2** – Attacco tra Kali e Metasploitable sulla stessa rete interna (gestita da pfSense), con scansione tramite msfconsole e nmap.
- **S07L3** – Uso del modulo `postgres_payload` sul servizio PostgreSQL di Metasploitable per ottenere una sessione Meterpreter.
- **S07L4** – Download e utilizzo di Tor Browser con impostazioni predefinite e navigazione sulla rete Tor; come bonus, installazione di Tails su macchina virtuale.
- **S07L5** – Exploit del servizio Java RMI (porta 1099) di Metasploitable per una sessione Meterpreter, con recupero della configurazione di rete e della tabella di routing della macchina remota.

## Settimana 9 – Log e threat intelligence

- **S09L4** – Creazione e gestione delle regole per i file di log di sicurezza in Windows tramite il Visualizzatore eventi (`eventvwr`).
- **S09L5** – Threat Intelligence e Indicatori di Compromissione (IOC): analisi di una cattura di rete con Wireshark per identificare gli IOC, ipotizzare i vettori d'attacco e suggerire contromisure.

## Settimana 10 – Amministrazione di sistema

- **S10L2** – Gestione dei permessi di lettura, scrittura ed esecuzione in Linux (`chmod`, `ls -l`) con relazione sulle scelte effettuate.
- **S10L4** – Esercizio teorico su cloud computing, backup e RAID: confronto dei principali provider (AWS, Azure, Google Cloud, ecc.) e dei modelli di servizio IaaS/PaaS/SaaS.
- **S10L5** – Gestione dei gruppi di utenti in Windows Server 2022: creazione di gruppi e assegnazione dei permessi, con riflessioni sulla sicurezza.

## Settimana 11 – PowerShell

- **S11L5** – Laboratorio sull'uso di Windows PowerShell: cmdlet, uso di `netstat` e gestione del Cestino da riga di comando.

## Nota

Materiale didattico prodotto a scopo di studio nell'ambito del corso. Tutte le tecniche e gli
strumenti documentati sono stati utilizzati esclusivamente in un ambiente di laboratorio isolato.
