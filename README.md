# Passo a passo inicial com a NodeMCU e a plataforma de IoT Thingspeak

Utilização da plataforma Thingspeak para o contexto de Internet das Coisas - https://thingspeak.com/

Os fields dentro do código se referem aos fields 1 e 2 dentro do Channel Settings na plataforma, assim, são mapeados:

                             String postStr = apiKey;
                             postStr +="&field1=";
                             postStr += String(t);
                             postStr +="&field2=";
                             postStr += String(h);
                             postStr += "\r\n\r\n";
                            
O apiKey é o token necessário para realizar a autenticação na API da plataforma e está nas configurações: API Keys do Thingspeak.
Dentro do Channel Settings, podemos adicionar mais fields, a fim de receber dados dos sensores:

![things1](https://user-images.githubusercontent.com/2284795/74734446-51f15d80-522d-11ea-9bfc-7ccf00a43026.PNG)

E, na parte do Private View, podemos adicionar as visualizações de acordo com os fields que escolhemos nas configurações:

![thingspeak](https://user-images.githubusercontent.com/2284795/74734608-a694d880-522d-11ea-8763-82a5f0b274a3.PNG)

Para configurar a integração com o Twett vá em Apps > ThingsTweet. Fará uma conexão com uma conta, e, posteriormente, há o código no arquivo (..)tweet.ino

![TWEET](https://user-images.githubusercontent.com/2284795/74780347-2ba7de00-527e-11ea-91da-e065be9e7e59.PNG)

Nos Apps > React, é possível criar uma reação caso haja um ou mais valores que precisam de controle: 

![Captura de Tela 2020-02-20 às 11 46 08](https://user-images.githubusercontent.com/2284795/74945969-578aa700-53d7-11ea-9fd9-de7282cfc081.png)




