# Relatório da Ponderada: Criação e Acesso a uma Instância EC2 

## 1. Introdução
Neste relatório, descrevo o processo de criação de uma instância EC2 na AWS e o acesso a essa instância usando SSH via PuTTY.

## 2. Objetivo
O objetivo deste experimento é demonstrar como criar uma instância EC2 na AWS e acessá-la remotamente via SSH.

## 3. Materiais
- Conta na AWS
- Computador com PuTTY instalado

## 4. Método
### 4.1 Criar uma instância EC2 na AWS:
1. O primeiro passo é realizar o login no [Console AWS](https://aws.amazon.com/console/).
2. Logo após, você irá para a aba "EC2" e vai clicar em "Launch Instance", para iniciar a criação de uma instância.
4. Siga as etapas do formulário, selecionando:
   - Nome da instância;
   - Sistema operacinal;
   - Configurações de rede.
5. Por fim, crie um par de chaves para autenticação SSH e salve as mesmas em um arquivo ppk para ser utilizado logo após no PuTTy

### 4.2 Acessar a instância EC2 via SSH usando PuTTY:
1. Abra o PuTTY.
2. No campo "Host Name (or IP address)", insira o IP público da instância.
3. Logo após, no menu à esquerda, vá para "Connection" > "SSH" > "Auth".
4. Navegue até a seção "Private key file for authentication" e selecione o arquivo.ppk da chave privada correspondente ao par de chaves utilizado na criação da instância EC2.
5. Volte à sessão "Session" no menu à esquerda e clique em "Open" para iniciar a conexão SSH.

## 5. Resultados
- [Captura de tela da instância criada](images/instanciacriada.jpg)
- [Captura de tela da instância criada - 2](images/instanciasendoexecutada.jpg)
- [Captura de tela incluindo detalhes da instância: IP da máquina EC2](images/detalhesdainstancia.jpg)
- [Captura de tela do acesso SSH bem-sucedido usando o PuTTY](images/instanciaconectada.jpg)
- IP da máquina EC2: `44.204.34.50`

## 6. Conclusão
Nesta ponderada, coloquei em prática os meus conhecimentos sobre como criar uma instância EC2 na AWS e acessá-la remotamente via SSH utilizando o PuTTY. Agora pude ter uma visão mais clara sobre a conexão destas ferramentas!
