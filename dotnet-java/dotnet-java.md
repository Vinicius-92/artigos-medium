Hello world.

Sendo minha primeira tentativa de escrever algo relacionado a tecnologia e primeiro post aqui no medium, acredito que não teria outra forma de começar a não ser com essas palavras.

O intuito dessa publicação é falar um pouco sobre a minha experiência aprendendo C# e .NET quando migrei do Java como minha stack principal, a minha experiência nesse momento não era profissional, apenas de estudos e com isso acredito que tive pontos positivos e negativos, pois não tinha nenhum conhecimento muito profundo que pudesse causar disparidade, entretanto também não tinha bases sólidas suficientes para fazer as relações entre tópicos que poderiam acelerar esse aprendizado. Ao entrar no mundo .NET tive o fortúnio de conhecer quando já estava em sua versão Core 3.1, que é da fase OpenSource da Microsoft e me permitiu desenvolver dentro do ambiente que já conhecia utilizando Linux e VSCode, quebrando qualquer dificuldade de aprender desenvolvimento em uma plataforma diferente do meu habitual e utilizando toolings que já me era familiar.

Agora vou abordar por tópicos as comparações que acredito fazerem sentido para quem pode estar no início de carreira se encontrando na mesma situação:

### Sintaxe

Quando analisamos a história de como surgiu o C#, independente de julgamentos, vemos que a linguagem surgiu como uma necessidade da Microsoft de ter sua própria "versão" do Java, que por conta de disputas relacionadas à licenciamentos não era possível, com isso temos duas linguagens que no seu início tinham o mesmo DNA, herdando estruturas e palavras muito similares, qualquer pessoa que conheça Java consegue ler um código C# e identificar diversos padrões, chegando até mesmo a entender e modificar sem muitos problemas.

![Screenshot](https://raw.githubusercontent.com/Vinicius-92/artigos-medium/main/dotnet-java/fib.jpg)

No meu primeiro contato com C# eu refiz alguns exercícios de lógica que me foram propostos no meu estágio, em questão de horas foi possível traduzir de uma linguagem para outra, apenas fazendo pesquisas pontuais quando a forma de implementar interfaces, definir encapsulamento dos atributos ou até o nome de algumas estruturas como Listas e Dicionários.
Devo confessar porém que olhando pra esse código hoje em dia ele não se parece com C# nos seus padrões mais comuns, era uma versão muito "Javaficada", porém rodava e atendia os requisitos de lógica e naquele momento era o que importava.

Tendo isso como base, tenho que dizer que na migração a sintaxe será um dos detalhes mais bem resolvidos logo de cara e com o tempo e repetição é fácil entender e pegar o jeito da linguagem.

### Ferramentas

No universo Java, o mais comum que temos na parte de ferramentas de edição de texto são as IDE's, mais especificamente Eclipse e Intellij, sendo a primeiro OpenSource e grátis e a segunda proprietária da JetBrains e contendo edição grátis e paga para features mais avançadas, com qualquer uma das duas é possível trabalhar muito bem e foi com elas que comecei no mundo da programação, costumo recomendar o Intellij por ter me identificado mais e também por ser mais bonito. 

Já no .NET o que temos como padrão de mercado seria o Visual Studio, tendo também a versão grátis e paga, além dela a JetBrains produz também o Rider, IDE paga para desenvolvimento em .NET. Além das citadas, graças a abertura de código por parte da Microsoft, foram desenvolvidas também formas de rodar, debuggar e gerar estruturas para desenvolvimento também fora das IDEs, através do dotnet cli (command line interface) e utilizado através do terminal, com isso até mesmo editores de texto comuns tem uso facilitado, com destaque o VSCode que com a utilização da cli e das extensões disponíveis se torna uma versão muito leve com funcionalidades básicas muito próximas de uma IDE.

Como citado no início do texto, comecei o desenvolvimento no ambiente que me era comum com Linux e VSCode, sendo assim ouve um nível um pouco maior de busca de soluções que são simplificadas com o uso de IDEs, como buscar e adicionar pacotes ao projeto, conexão com banco de dados e outras ferramentas que não vem por padrão no editor de texto, porém isso não chega a ser impeditivo e acaba agregando em conhecimento e aprendizado de como pesquisar e buscar soluções. Tendo dito isso, recomendo pra quem quiser um caminho mais simples ir diretamente para o Visual Studio na versão grátis, que poderá facilitar esse primeiro momento.

Hoje utilizo o Rider e por conta da proximidade com as ferramentas da JetBrains me tornou muito mais produtivo e retirou esses pequenos pontos de falta de ferramentas incluídas no pacote, mas para edições rápidas e alguns projetos paralelos a leveza do VSCode ainda me atrai.

Na escolha de qualquer uma dessas opções, a utilização será bastante tranquila, as ferramentas de refatoração e autocomplete irão auxiliar em muito na construção dos projetos de estudo.

### Conteúdo técnico disponível

Chegando nesse ponto é onde começamos a ter um maior nível de disparidade entre as duas plataformas, por conta do tempo maior em que Java possui comunidades abertas e quantidade maior em projetos ao redor do mundo, o conteúdo técnico produzido para linguagem, soluções de problemas e dúvidas, e conteúdos úteis em geral serão mais fáceis de serem encontrados. Acredito que seja incrivelmente improvável não encontrar soluções para problemas que você encontra durante o desenvolvimento.

Já a comunidade .NET open source é bem mais recente e por conta da quantidade menor de projetos em desenvolvimento e no ar, principalmente da versão multiplataforma, é possível se deparar com problemas não encontrados por outros e ainda não desbravados, ou também que somente com a documentação oficial pessoas iniciantes não tenham a facilidade de solucionar sozinhas.

Falando em documentação ambas possuem documentações oficiais vastas e completas, entretanto nesse quesito acredito que a Microsoft saia na frente com documentações de simples entendimento, em sua grande maioria disponíveis também em Português, eles também produzem artigos, vídeos, tutoriais e muitos mais materiais oficiais com qualidade e acessíveis para todos os níveis de conhecimento.

### Componentes, Interfaces, Frameworks e etc

Quanto se trata do ecossistema como um todo de cada plataforma, ambos são extremamente maduros e continuam evoluindo desde suas criações, hoje em dia acredito que nessa parte o .NET tem tido mais sucesso em evoluir mais rapidamente como um todo e trazer features interessantes para a linguagem, porém o Java tem cada vez mais se modernizando e são linguagens extremamente diferentes de quando começaram e que apesar de terem saído do mesmo ponto, hoje se diferem mais em escolhas de como resolver problemas. Temos o exemplo das Collections Streams em Java para o LINQ em C#, que são formas de lidar com coleções de diferentes tipos de dados e estruturas de listas, no Java essa melhoria veio com a versão 8 em 2014, enquanto o LINQ já faz parte do .NET desde 2007.
Apesar das diferenças em sintaxe, entendendo o conceito lógico de uma a outra se torna extremamente simples de implementar, eu não compreendia completamente o conceito de streams em Java, porém após aprender a realizar as operações com LINQ ao retornar ao Java consegui utilizar os streams de forma muito fluída.

![Screenshot](https://raw.githubusercontent.com/Vinicius-92/artigos-medium/main/dotnet-java/linq.jpg)

### Conclusão

A migração de uma linguagem para outra é muito menos onerosa de que para outras linguagens, então se ocorrer a necessidade dado escopo do projeto ou vaga de interesse, pode ser uma boa estratégia conhecer um pouco da plataforma .NET pois sabendo Java e as bases de lógica de programação já temos um grande caminho percorrido para produzir soluções similares em C#.
Lembrando que isso é a visão da minha experiência e pode não refletir a realidade de muitos, porém caso esteja nesse limiar de troca entre Java e C#, espero que de alguma forma esse compartilhamento de ideias possa ser útil.
