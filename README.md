# Dio_medusa_kali
Projeto prático utilizando Kali linux e Medusa

 

# Sobre o projeto

Configurar o ambiente: duas VMs (Kali Linux e Metasploitable 2) no VirtualBox, com rede interna (host-only).

Executar ataques simulados: força bruta em FTP, automação de tentativas em formulário web (DVWA) e password spraying em SMB com enumeração de usuários.
















# Tecnologias utilizadas

## Sistema Operacional
- Linux Kali
- Shell Linux

## Programa usado 
- Medusa
- Nmap



Tela inicial do Metasploitable necessário login e senha, por padrão msfadmin para ambos<img width="724" height="401" alt="Captura de tela em 2025-11-29 01-19-41" src="https://github.com/user-attachments/assets/a87baeec-4bbc-4b0f-9a6c-018289ccfef7" />


Identificando numero IP da maquina vulneravel e tirando um snapshot, caso precise recuperar <img width="1222" height="411" alt="Captura de tela em 2025-11-29 00-29-36" src="https://github.com/user-attachments/assets/82f6ba2c-c43b-4a90-b5ba-2dcef8a03f2d" />


já no kali linux no terminal, iremos digitar o comando  ping -c 3  para se comunicar com metasploit<img width="662" height="509" alt="Captura de tela em 2025-11-29 01-27-05" src="https://github.com/user-attachments/assets/471bf890-ff47-43a0-8fed-3e3bfd36ac54" />

O cenário a ser explorado é de um servidos FTP antigo, que pode estar com falha de segurança, 
o objetivo aqui é confirmar se existe alguma vunerabilidade
o parâmetro -sV ele tenta identificar, a versão do serviço que está rodando em cada porta
na imagem podemos ver que todas as portas estão abertas, e na coluna ao lado os serviços e versões
<img width="1065" height="380" alt="Captura de tela em 2025-11-29 03-11-51" src="https://github.com/user-attachments/assets/e276a322-7b78-4865-bdbf-c386ed56fb2c" />





git@github.com:koanjazz/Dio_medusa_kali.git

``` bash

## Metasploitable 2
(MSF2) é uma máquina virtual Linux intencionalmente vulnerável, criada para testes,
demonstrações e prática em segurança ofensiva.
Ele é baseado no Ubuntu 8.04 LTS Server, com pacotes propositalmente:

desatualizados,

mal configurados,

rodando serviços inseguros por padrão.

Ou seja: é um ambiente controlado para exploração.

| Serviço               | Porta   | Problema Técnico                              |
| --------------------- | ------- | --------------------------------------------- |
| **vsftpd 2.3.4**      | 21      | Backdoor presente no código fonte             |
| **OpenSSH antigo**    | 22      | Não vulnerável, mas permite brute-force       |
| **Distcc**            | 3632    | Execução remota de comandos (RCE) sem auth    |
| **Samba 3.0.20**      | 139/445 | Exploit "username map script" (CVE-2007-2447) |
| **Telnet**            | 23      | Autenticação fraca + plaintext                |
| **MySQL**             | 3306    | Credenciais default + permissão ampla         |
| **Tomcat 5.5**        | 8180    | Credenciais padrão + upload de WAR            |
| **ProFTPD**           | 2121    | Backdoor da versão comprometida               |
| **Apache/PHP antigo** | 80      | Vários CVEs de deserialização / RCE           |


-----------------------------------------------------------------------------------

##  ping
é uma ferramenta que testa conectividade de rede usando o protocolo ICMP (Internet Control Message Protocol), especificamente:

ICMP Echo Request (tipo 8)

ICMP Echo Reply (tipo 0)

Ele mede:

latência (tempo de ida e volta — RTT)

perda de pacotes

disponibilidade da máquina remota










