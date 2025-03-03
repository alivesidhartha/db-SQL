# Домашнее задание к занятию «Резервное копирование баз данных» - Макану Александр


### Задание 1

Разрешённые сетевые службы:

FTP (vsftpd 2.3.4)
SSH (OpenSSH 4.7p1)
Telnet
SMTP (Postfix smtpd)
DNS (ISC BIND 9.4.2)
HTTP (Apache 2.2.8)
Samba (smbd 3.X - 4.X)
MySQL (MySQL 5.0.51a)
PostgreSQL (8.3.0 - 8.3.7)
VNC (протокол 3.3)
UnrealIRCd (3.2.8.1)
Apache Tomcat (5.5)
NFS (2049/tcp)

Найденные уязвимости:

1. vsftpd 2.3.4 Backdoor (CVE-2011-2523)
Exploit: https://www.exploit-db.com/exploits/49757

2. Samba smbd 3.x Remote Code Execution (CVE-2007-2447)
Exploit: https://www.exploit-db.com/exploits/16320

3. UnrealIRCd 3.2.8.1 Remote Command Execution (CVE-2010-2075)
Exploit: https://www.exploit-db.com/exploits/13853

### Задание 2

SYN-сканирование (-sS) отправляет SYN-пакеты и ждет ответа. Если порт открыт, сервер отвечает SYN-ACK, если закрыт — RST.

FIN-сканирование (-sF) отправляет FIN-пакеты. Открытые порты игнорируют запрос, закрытые отвечают RST.

Xmas-сканирование (-sX) отправляет FIN, PSH и URG-пакеты. Реакция такая же, как при FIN-сканировании.

UDP-сканирование (-sU) отправляет UDP-пакеты. Если порт закрыт, сервер отвечает ICMP "Port Unreachable". Если открыт, ответа может не быть.