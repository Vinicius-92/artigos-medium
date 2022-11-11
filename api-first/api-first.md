Introdução - falar workshop 

 
 

No início desse ano tive a oportunidade junto com um colega de trabalho a realizar um workshop para empresa que estamos alocados através de consultoria pra falar sobre boas práticas de envolvimento de APIs e do conceito de API-First, essa era uma demanda do cliente que enxergava as os benefícios que isso poderia trazer para a cultura interna da empresa, vamos juntos entender um pouco mais sobre essa abordagem. 

 
 

O que é uma API? 

 
 

Só para termos registrado aqui o conceito de API para facilitar o quê abaixo que vamos tratar, API é um acrônimo para Application Programming Interface ou Interface de Programação de aplicações, esse nome para um iniciante pode ser bastante abstrato e confesso que demorei muito tempo depois de ter escrito minha primeira API para de fato entender o que ela era, a API nada mais é do que um contrato que define o que vai ser solicitado e retornado em cada chamada. 

Tá, mas ainda não está bom, vamos lá, suponhamos que você queira usar uma calculadora de mão, todos os meios que você tem de interagir com ela são um contrato que conhecemos sem pensar muito nisso. Porque o x ou asterisco é multiplicação? Não existe um motivo lógico, mas nós sabemos que assim ele funciona e usamos dessa forma, como a calculadora vai processar isso e entregar o resultado não é importante, a única coisa que importa pra quem pede a informação é o resultado de 10 x 5, isso é um contrato. 

Agora que entendemos que a API é o meio do caminho entre o que enviamos e o que recebemos, vamos entender melhor porque devemos pensar nesse contrato antes de pensar em como ele vai resolver o problema.  

 
 

O que é API-First? 

 
 

API-First é o uma abordagem de desenvolvimento de software que coloca em primeiro lugar as APIs, antes de qualquer implementação, já definimos todos os contratos de requisição e resposta, deixamos tudo padronizado e documentado. 

A partir do momento que temos esse contrato, podemos começar a trabalhar para os dois lados da API, de quem consome ou produz os resultados, mesmo sem que qualquer um dos lados tenha conhecimento dos detalhes do outro, obedecendo o contrato não corremos o risco de qualquer incompatibilidade, assim, todos podem trabalhar simultaneamente para acelerar o time-to-market da solução e isso tem potencial de gerar retornos mais rápidos. 

 
 

Mas como funciona esse paralelismo? 

 
 

Como existe a possibilidade de começar o desenvolvimento independente da implementação, os consumidores, sejam eles front-end, back-end, mobile, parceiros ou todos os anteriores, já sabem qual será a entrega realizada e com isso conseguem desenvolver suas soluções pensando no projeto pronto enquanto você consegue preparar a sua solução ao mesmo tempo para entregar aquilo que foi apresentado na documentação de sua API. Isso nos traz o benefício de conseguir atender melhor a prazos e conseguir manter uma qualidade produzida superior. 

 
 
 

(slide porque utilizar + benefícios) 

 
 

Necessidade de boas práticas 

 
 

Um ponto muito importante de salientar é a necessidade de aplicar boas práticas na definição da sua API, um contrato que não esteja muito bem definido e documentado extensivamente não vai ajudar a quem consome, pois exigirá comunicação frequentemente para esclarecer pontos que deveriam estar descritos de maneira assíncrona através da documentação. Seguir conceitos como REST e RESTful são extremamente indicados, por serem o padrão atual do mercado, é mais fácil para ser entendido por qualquer time que irá trabalhar no processo. 

 
 

Ferramentas de suporte ao API First. 

 
 

Algumas ferramentas de suporte que temos para essa abordagem seria o OpenAPI e Swagger para gerar e compartilhar com maior facilidade todos os detalhes do contrato da API, podemos considerar que esse padrão de especificação é o mais adotado pelo mercado e é difícil falar de API sem pensar nele. 

Outra ferramenta muito interessante quando se trata de API First são os mocks, que é uma forma de criar retornos padrão com base no nosso contrato estabelecido para que com isso nossos consumidores já tenha um retorno padrão para nossos endpoints e podendo assim começar a testar, existem diversos sites que oferecem isso gratuitamente e um deles é o Mocky (https://designer.mocky.io/). 

 
 

Diferentes abordagens de código x yaml 

 
 

Quando falamos do documentar nossas APIs com OpenAPI existem duas abordagens mais comuns que podemos utilizar para gerar esses arquivos, que no final são apenas arquivos JSON ou YAML que é interpretado e é possível visualizar com a UI no Swagger Editor (https://editor.swagger.io/), essas abordagens são: gerar o arquivo através do código ou gerar o código com base nesse arquivo escrito diretamente na sintaxe desejada. Como cada um deles funciona? 

 
 

Gerar código com base no arquivo: 

Com uso do site citado acima para editar arquivos Swagger ou até com extensões do VsCode podemos escrever diretamente em YAML os detalhes que serão utilizados em nossa API, exige um pouco de prática, porém assim que se pega o jeito o formato é bastante simples e repetitivo, facilitando a escrita. Através dele existem ferramentas que facilitam a geração do código em diversas linguagens, como o Java, por exemplo. 

 
 

Gerar arquivo através do código: 

Uma abordagem que eu prefiro e recomendo, é gerar a especificação OpenAPI através do código, através de pacotes e anotações utilizadas em nosso código, é possível que ao realizar o build de nossas aplicações seja gerado esse arquivo sem a necessidade de interagir com ele de outra forma. Eu recomendo essa abordagem pois deixa o código e a documentação atreladas e dessa forma não corremos o risco de em próximas atualizações termos dois pontos diferentes para manter sincronizados e assim termos um ponto de falha em casa de erro no processo, além disso, possibilitando que o próprio código seja mais fácil de ser trabalhado por novas pessoas que entrem no projeto pois já ter uma documentação disponível de maneira fácil e acessível. 

 
 

Espero que essa introdução tenha sido interessante pra você e vou deixar abaixo um repositório onde tenho os slides, referências e projeto em .NET que usa essa implementação do API First. 

 
 

URL Git - https://github.com/Vinicius-92/workshop-api-first 

 