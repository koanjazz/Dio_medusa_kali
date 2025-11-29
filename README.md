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
Técnicamente, ele funciona usando o protocolo ICMP (Internet Control Message Protocol).








