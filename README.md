# thingspeack-iot

Utilização da plataforma Thingspeak para o contexto de Internet das Coisas - https://thingspeak.com/

Os fields dentro do código se referem aos fields 1 e 2 dentro da plataforma, assim, são mapeados:

                             String postStr = apiKey;
                             postStr +="&field1=";
                             postStr += String(t);
                             postStr +="&field2=";
                             postStr += String(h);
                             postStr += "\r\n\r\n";
                            
Dentro do Channel Settings podemos adicionar mais fieds, a fim de receber dados dos sensores.

O apiKey é o token necessário para realizar a autenticação na API da plataforma e está nas configurações do Thingspeak.

