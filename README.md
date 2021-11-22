# Request-Forwad

Request forwad direciona mensagens de um **Host Remoto** para um **Host Local** fazer as requisições usando sua rede.
 
 - _**Host Local :**_ Host local é o dispositivo responsável por efetuar de fato as requisições solicitadas pelo _**Host Remoto**_ ao _**Servidor Alvo**_.

 - Host remoto: Dispositivo que deseja fazer requisições ao _**Servidor Alvo**_ usando a conexão do _**Host Local**_
 
 - Servidor de Redirecionamento: Servidor responsável por encaminhar as mensagens do _**Host Remoto**_ para o _**Host Local**_ enviar ao _**Servidor Alvo**_.
 
 - Servidor Alvo: Servidor que o _**Host Remoto**_ deseja enviar mensagens utilizando uma conexão feita pelo _**Host Local**_.
 
 
**Host Remoto** | **Servidor de redirecionamento** | **Host local** | **Servidor Alvo** 
----------- | ---------------------------- | ----------- | ---------------
Envia requisicao para o _**Host local**_ fazer -> | (Espera conexão do _**Host Local**_ e do _**Host Remoto**_) | <- Se conectar ao _**Servidor de redirecionamento**_ para esperar mensagens | (Espera conexão de algum host)
 (Espera Resposta) | Recebe mensagem do _**Host Remoto**_ e direciona ao _**Host local**_ -> | Recebe mensagem do _**Servidor de Redirecionamento**_ e direciona ao _**Servidor Alvo**_ -> | Recebe e processa a requisição
Processa a mensagem como deseja | <- Direciona a mensagem do _**Servidor alvo**_ ao _**Host Remoto**_ que solicitou a requisição. | <- Recebe e envia a resposta ao _**Servidor de redirecionamento**_ | <- Envia resposta ao _**Host Local**_
 
                                            
