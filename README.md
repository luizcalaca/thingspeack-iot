# Passo a passo inicial com a NodeMCU e a plataforma de IoT Thingspeak

Utilização da plataforma Thingspeak para o contexto de Internet das Coisas - https://thingspeak.com/

Os fields dentro do código se referem aos fields 1 e 2 dentro da plataforma, assim, são mapeados:

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

Para configurar a integração com o Twett vá em Apps > ThingsTweet

![TWEET](https://user-images.githubusercontent.com/2284795/74780347-2ba7de00-527e-11ea-91da-e065be9e7e59.PNG)



