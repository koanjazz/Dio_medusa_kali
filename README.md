# Dio_medusa_kali
Projeto prático utilizando Kali linux e Medusa


[![NPM](https://img.shields.io/npm/l/react)](https://github.com/koanjazz/Dio_medusa_kali/blob/main/LICENSE) 

# Sobre o projeto

Configurar o ambiente: duas VMs (Kali Linux e Metasploitable 2) no VirtualBox, com rede interna (host-only).

Executar ataques simulados: força bruta em FTP, automação de tentativas em formulário web (DVWA) e password spraying em SMB com enumeração de usuários.














## Layout mobile
![Mobile 1](https://github.com/acenelio/assets/raw/main/sds1/mobile1.png) ![Mobile 2](https://github.com/acenelio/assets/raw/main/sds1/mobile2.png)

# Tecnologias utilizadas

## Sistema Operacional
- Linux Kali
- Shell Linux

## Programa usado 
- Medusa

Identificando numero IP da maquina vulneravel e tirando um snapshot, caso precise recuperar <img width="1222" height="411" alt="Captura de tela em 2025-11-29 00-29-36" src="https://github.com/user-attachments/assets/82f6ba2c-c43b-4a90-b5ba-2dcef8a03f2d" />


```bash


git@github.com:koanjazz/Dio_medusa_kali.git

# Entrando na maquina vulnerável Metasploitable 2

#Primeiro passo:
o Metasploit vai pedir um login e uma senha
por padrão, a senha deverá ser msfadmin para login e senha

#Segundo passo:
Identificar o numero de IP do metasploit
com o comando (ip a), identificando o numero de IP, que muito provavelmente será (129.168.56.102)
já teremos o nosso alvo e maquina vulnerável

#Terceiro passo:
Agora no kali, vamos testar a conexão do nosso sistema com o metasploit, com o comando ping -c 3  seguido do IP
da maquina alvo (192.168.56.102)
#NOTA: Ping é uma ferramenta de rede usada para testar a conectividade entre um dispositivo e outro na Internet ou rede local.
Tecnicamente, ele funciona usando o protocolo ICMP (Internet Control Message Protocol).








