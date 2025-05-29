das-1-2025
Aula dia 26/02
Livro ENG SOFT MODERNA CAP-07 https://engsoftmoderna.info/cap7.html
Interface, pacotes, componentes, modulos, camadas, serviços O pacote ajuda na arquitetura de software deixando o projeto mais organizado, eficiênciente, com o objetivo de criar um software de mais alto nível Camada de apresentação (front) Camada de gerir informação (back) Camada de informação (bd,drivers, devices) Anotação são tipos de componentes, são bibliotecas, feitas de antemão, e usadas para facilitar na programação No Java se refere como @ Httpserveletrequest (Java) ajuda a entender oq è o Java vindo da internet

Aula dia 27/02
Padrões aquiteturais, umas das mais utilizadas é em camadas. Basica front / back / bd

Aquitetura model view-controlle ou MVC

view: apresentação dos dados ao usuario

model: acessar e gerenciar dados

controller: controlar a tela

entidade:

modelo: outra classe que representa os dados que vão para outra tela

Microsserviços: pode ser um modulo, ideia que nao tenha interface grafica. Api rest. Deve ter camadas.

Monolito

Repositorio unico de codigo
Uso de uma unica tecnologia padrão
Compilado, testado, unico pacote
Deploy com um unico sistema
Executado como um unico processo no sistema operacional
Unico banco de dados
Aula dia 05/03
Padrão arquitetural: solução para um problema especifico.

MVC: separa as responsabilidades (model(dados) - view(tela) - control(comportamento))

Estilo arquitetura = organização do projeto

Arquitetura em camadas

DIvisão de responsabilade

Perfomace

Segurança

Manutenibilidade

Camada de apresentação

Requisitos próprios
Camada de logica de negocio (aplicação)

Local central para definiição e atualização de regras
Escalar o backend suportar as requisições
Camada de persistência

Banco de dados relacional - consolidada
Resolve problemas de concorrencia
Permite compartilhamento de dados
Aula dia 06/03
Who Needs an Architect ? https://martinfowler.com/ieeeSoftware/whoNeedsArchitect.pdf
O que é arquitetura?

A arquitetura de um sistema de software(em um dado ponto no tempo) é sua organização ou estrutura de componentes significativos interagindo por meio de interfaces, esses componentes sendo compostos de componentes e interfaces sucessivamente menores
Qual o comportamento do arquiteto da "Matrix"?

Aquele quem toma as decisões mais importantes, logo no início do projeto, para que todos tenham um plano a seguir, sendo o único responsável por garantir a integridade conceitual de um sistema
Qual o comportamento do arquiteto ideal?



É orientar a equipe de desenvolvimento, levantar seu nível para que possam assumir questões mais complexas. Melhorar a habilidade da equipe de desenvolvimento dá ao arquiteto uma alavancagem muito maior do que ser o único tomador de decisões e, portanto, correr o risco de ser um gargalo arquitetônico.
Aula dia 13/03
-U arquiteto tem, em comparação com as de um desenvolvedor. Como mostrado no diagrama, um arquiteto é responsável por coisas como analisar os requisitos comerciais para extrair e definir as características da arquitetura (os “atributos”), selecionar quais padrões e estilos da arquitetura se encaixariam no domínio do problema e criar componentes (blocos de construção do sistema). -Para que a arquitetura funcione e preciso que o desenvolvedor e o mesmo se comuniquem para o projeto ser um sucesso.


Aula 10/04/2025
Nessa aula vamos continuar o capítulo do livro nesta página

Configurabilidade -> Dá pra configurar como quer
Extensibilidade -> Dá pra aumentar as funcionalidades (tipo VS Code com as extenções das linguagens)
Instabilidade -> Facilidade de instalar
Aproveitamento/reutilização -> Poder confiar
Localização -> Suporte aos LOCALEs
Manutenção -> Manutenabilidade
Portabilidade -> Rodar bem em diferentes plataformas
Suporte -> Definir o nível que precisa de suporte
Atualização -> A capacidade de atualizar com facilidade/rapidez

🧠 Aulas dos dias 10/04/2025, 23/04/2025 e 24/04/2025
📄 Atividade 1.1 - Resumo sobre Características Arquiteturais
Quando uma empresa decide criar um software, é feita uma lista de tudo o que esse sistema precisa fazer (os famosos requisitos). Só que o arquiteto de software precisa pensar em coisas que vão além dessas funções visíveis.

Apesar de o arquiteto poder ajudar com essas funções, sua responsabilidade principal é pensar e definir tudo que o sistema precisa fazer além das funcionalidades básicas, ou seja, o que está “por trás dos panos”.

O que é uma característica arquitetural?
Ela precisa seguir 3 regras:

Ser sobre algo fora do que o software faz diretamente (algo fora da funcionalidade comum).

Influenciar como o sistema vai ser desenhado internamente.

Ser essencial ou muito importante para que o software funcione bem.

Tipos de características arquiteturais:
Operacionais – São relacionadas a como o sistema funciona na prática. Exemplos:

Disponibilidade (estar no ar quando for necessário)

Continuidade (conseguir continuar rodando mesmo com problemas)

Desempenho (ser rápido e eficiente)

Recuperação (voltar ao normal depois de erros)

Confiabilidade (não falhar)

Segurança, robustez e escalabilidade (aguentar mais usuários ou dados sem travar)

👉 Essas foram discutidas na aula do dia 09/04 em mais detalhes.

Estruturais – Falam sobre como o código é organizado. Exemplos:

Facilidade de configurar ou mudar

Possibilidade de aproveitar e reutilizar código

Manutenção (fácil de corrigir ou melhorar)

Portabilidade (funcionar em diferentes sistemas)

Suporte técnico (tema sensível, principalmente se você trabalha com isso!)

Atualização (poder ser atualizado com facilidade)

Transversais – São mais difíceis de classificar, mas são igualmente importantes. Exemplos:

Acessibilidade (uso por pessoas com necessidades especiais)

Armazenamento, autenticação, autorização

Legalidade, privacidade, usabilidade e viabilidade (possibilidade real de existir e ser usado)

💡 Importante: Qualquer lista de características nunca será completa. Cada software pode ter necessidades muito específicas. Por exemplo, no caso de um sistema usado na Itália, pode ser necessário garantir certos padrões de disponibilidade e recuperação só para aquele país.

Dicas importantes para arquitetos:
Evite definições confusas ou soluções que parecem servir para tudo.

Nunca tente fazer a arquitetura “perfeita”, mas sim a “menos pior” possível.

🎮 Metáfora legal: Pense na arquitetura como a build de personagem em um jogo tipo Elden Ring. Você não consegue deixar todos os atributos no máximo. Então, precisa escolher o que é mais importante e aceitar os compromissos (os famosos trade-offs).

🌀 Iteração é chave: Assim como no desenvolvimento de software, a arquitetura também precisa ser revista e melhorada ao longo do tempo.

📄 Atividade 1.2 - Resumo sobre Fundamentos da Arquitetura de Software
Os estilos ou padrões de arquitetura mostram como as partes do sistema se relacionam. Eles servem como base para conversas e decisões sobre a arquitetura. Por isso, é essencial que os arquitetos conheçam bem esses modelos.

Exemplos de estilos de arquitetura:
Grande Bola de Lama (Big Ball of Mud)
Quando o sistema não tem nenhuma organização clara. É um tipo de antipadrão (ou seja, algo que geralmente devemos evitar). Mesmo assim, é muito comum na vida real.

Arquitetura Unitária
Quando o software roda inteiro em um único computador. Era mais comum no passado.

Cliente/Servidor
Divide o sistema em duas partes:

O cliente (quem usa, como um navegador ou aplicativo)

O servidor (quem processa e responde)

Exemplos:

Computador + Servidor de banco de dados

Navegador + Servidor web

Sistema em três camadas (ex: banco de dados, servidor de aplicação, cliente)

Arquiteturas Monolíticas vs Distribuídas
Monolítica: Tudo junto em um só lugar (como em camadas, pipeline ou microkernel)

Distribuída: As partes do sistema rodam separadas, comunicando-se via rede. Exemplos:

Arquitetura baseada em serviços (como microserviços)

Orientada a eventos

👉 Apesar de serem poderosas, as arquiteturas distribuídas têm desafios, descritos nas falácias da computação distribuída:

A rede é confiável (spoiler: não é)

A latência (tempo de resposta) é zero (não mesmo)

A largura de banda é infinita (sonha)

A rede é segura (risos)

A topologia nunca muda (mas muda sim)

Existe só um administrador (muitas vezes o responsável some ou muda)

A rede é homogênea (na prática, é cheia de diferenças)

Considerações finais:
Analisar registros (logs) para entender erros é difícil, pois pode ter muitos eventos interligados.

Transações distribuídas (que envolvem várias partes do sistema ao mesmo tempo) complicam a consistência dos dados.

Outro desafio é manter e versionar o contrato, que é o acordo entre cliente e servidor sobre como os dados devem ser trocados.

Aula 26/02/2025
Livro Eng Soft Moderna - Cap 7

É a representação de mais alto nível do software

Por exemplo, pode ter uma camada de apresentação (front-end) e gerenciamento (back-end) e o banco de dados

Em alguns casos essa camada do front-end e back-end estão em um projeto só

Pacote = conjunto de código, uma indicação para novos devs entenderem onde vai cada coisa

É importante organizar as coisas, é interessante ter um padrão, não precisa reinventar
Entenda o porque das coisas na sua empresa, qual padrão decidiram fazer
Componentes -> São pequenas partes de código reutilizáveis

HttpServeletRequest -> Java entende pacotes vindos via rede por ele

Modulos -> Parte de um sistema com finalidade especificada

Interfaces -> Pontes de conexão entre módulos

Serviços -> São utilidades para o sistema

📅 Aula – 07/05/2025
🎉 Começamos o segundo bimestre! 🦭🦭🦭

🧱 Tema da aula: Estilo de Arquitetura Pipeline
Hoje aprendemos sobre um tipo de arquitetura chamado Pipeline, muito usado em sistemas Linux. Esse estilo surgiu na época dos sistemas Unix.

A ideia principal do pipeline é montar uma sequência (ou cadeia) de pequenos programas, onde cada um processa uma parte dos dados e passa o resultado para o próximo. É como uma linha de montagem: cada etapa faz uma parte do trabalho.

💻 Exemplo prático
O professor mostrou um exemplo de uso da arquitetura pipeline imitando o funcionamento do Linux, usando uma interface de linha de comando (CLI).

Ele utilizou o Git Bash, que é um terminal usado no Windows, para demonstrar como os comandos de terminal trocam informações entre si usando o símbolo de pipe (|).

🛠️ Comandos explicados
Durante a aula, o professor também explicou os comandos listados no livro, que são usados para:

Pesquisar dados

Filtrar informações

Exibir resultados, como no comando more, que mostra o conteúdo aos poucos

Aula 28-05-2025
Estilo de arquitetura baseada em Serviços
É uma combinação do estilo microsserviços e é considerada das mais pragmáticas, em grande parte pela flexibilidade sem ter tanta granularidade e aumentar a dificuldade de orquestrar. Embora seja distribuida ela não tem a mesma complexidade e custo.

Topologia
Segue a macroestrutura em camadas e consiste numa interface separada e serviços gerais remotos e separados. Na maioria dos casos existe apenas uma instância de cada serviço do domínio dentro de uma arquitetura baseada em serviços. Mas podem haver mais para fatores de escala e tolerância.

Serviços são acessados remotamente através de uma IU usando um protocolo de acesso remoto, embora REST seja usado geralmente, SOAP e RPC também pode ser usados pra consumir.

Variantes de topologia
Podem haver pontos diferentes de UI acessando diferentes serviços, isso possibilita a separação dos bancos de dados em bancos específicos do serviço.

É uma boa prática para fins de segurança isolar interações de validação da interface do usuário com uma camada de API (proxy ou gateway).

Design de serviços e granularidade
Serviços geralmente são granulares e cada serviço costuma ser projetado usado um estilo que consiste em uma camada fachada da API, camada comercial e camada de persistência

Outra abordagem é cada domínio usar sudomínios semelhantes a monolítica.

Trade-offs entre serviço e microsserviços:

SOA:

Prós: Maior controle e consistência de dados

Contras: Uma mudança no serviço pode exigir retestar e reimplantar um serviço miaor

Microsserviços:

Prós: Menor impacto de mudanças pelos serviços serem isolados

Contras: Maior complexidade na orquestração

Particionamento do Banco de Dados
Em serviços, embora não requerido, os serviços compartilham o banco de forma semelhante a arquitetura monolítica.

Os arquivos das classes que modelam os dados fazem parte de uma biblioteca compartilhada entre os serviços. Elas também podem contar código SQL.

Problema com isso é que alterar o SQL por exemplo pode afetar a estrutura de serviços que nem sequer usavam aquela tabela.

Uma técnica pra mitigar isso é particionar de forma lógica por meio de bibliotecas compartilhadas e federais.

A arquitetura baseada em serviços é particionada por domínio, sua estrutura orientada por domínio, não por consideração técnica.

Quando usar esse estilo de arquitetura
É um estilo pragmático, é natural ao fazer design orientado a domínios, pode ser usada pois preserva melhor as transações ACID do que qualquer outra arquitetura distribuida. É uma boa escolha para ter um nível de modularidade arquitetural sem entrar em armadilhas de granularidade excessiva.

Aula – 29/05/2025
Tema: Estilo de Arquitetura Microsserviços
Hoje estudamos microsserviços, um estilo de arquitetura que está bem na moda (com razão, é muito falado mesmo).

Um pouco de história
Diferente de outros estilos que surgem na prática e só depois recebem um nome, o termo “microsserviços” apareceu antes de ser amplamente usado, em um post do Martin Fowler e James Lewis chamado "Microser", publicado em março de 2014.

Base Conceitual
Esse estilo foi muito inspirado no Domain Driven Design (DDD), principalmente na ideia de contexto delimitado. Isso quer dizer que cada parte do sistema (serviço) funciona independente das outras, com seu próprio código e banco de dados, sem precisar compartilhar tudo com o resto – ao contrário de um sistema monolítico.

Primeira lei da arquitetura: trade-offs
Se você quer menos dependência entre as partes, vai acabar tendo que duplicar código em alguns casos – não dá pra reaproveitar tudo.

Em outras palavras: é como se cada microsserviço fosse um mini-sistema monolítico, mas todos se conectam para formar um sistema completo.

Arquitetura distribuída
Cada microsserviço roda separado, em seu próprio processo, máquina virtual ou container. Com isso, cada um pode ter sua infraestrutura própria.

O problema é que a performance pode cair, já que os serviços precisam se comunicar via rede, o que gera atraso (latência).

Contexto Delimitado
Cada serviço deve ter tudo o que precisa para funcionar sozinho, sem depender de outros. Essa ideia guia muitas decisões na hora de projetar o sistema.

Granularidade
A dúvida comum é: quão pequeno deve ser um microsserviço?

Às vezes os arquitetos erram e criam serviços pequenos demais, que precisam de vários outros para funcionar. Isso torna o sistema mais lento e difícil de manter.

Lembrete:

“Microsserviço” é só um nome, não precisa ser “micro” de verdade — Martin Fowler.

Dica de design:
Defina o tamanho com base na função e no domínio do serviço, observando as relações entre as partes e como os processos são feitos. Se forem muitos passos, talvez seja melhor unir serviços para evitar lentidão desnecessária.

Isolamento de dados
Cada microsserviço deve ter seu próprio banco de dados. Isso ajuda a manter a independência entre eles.

É importante planejar bem como dividir os dados, garantindo que cada parte seja a “dona” da sua informação. Além disso, pode-se escolher ferramentas diferentes para cada serviço, inclusive pensando no custo-benefício.

Camada de API
A API de um serviço não deve virar um controlador central da interface do usuário (UI). Ela serve para manter o limite de responsabilidade bem claro.

Reutilização operacional
Você pode sim reaproveitar funcionalidades entre microsserviços, desde que não crie dependência entre eles. O segredo é componentizar bem.

Front-ends
O front-end pode ser um monolito ou pode seguir a ideia de microfrontends. Porém, é mais difícil separar bem as partes no front-end do que no back-end.

Comunicação entre serviços
O arquiteto precisa decidir entre dois tipos de comunicação:

Síncrona: responde na hora

Assíncrona: envia uma mensagem e continua, esperando a resposta depois

Microsserviços costumam usar tecnologias diferentes entre si (poliglotas) e precisam saber se comunicar entre si, mesmo sendo diferentes. Isso é chamado de interoperabilidade.

Coreografia vs Orquestração
Coreografia:
Os serviços se comunicam sozinhos, sem ninguém mandando. Eles reagem a eventos. Isso deixa tudo mais solto, mais flexível. Mas, se o processo for muito complexo, os serviços podem ficar sobrecarregados tentando se coordenar.

Orquestração:
Um serviço central cuida do “roteiro” de como as partes vão se comunicar. É mais organizado, fácil de controlar e tratar erros. Mas cria mais acoplamento (as partes ficam mais dependentes umas das outras).

A escolha entre os dois depende do equilíbrio entre controle e flexibilidade.

Transações e Sagas
Fazer transações entre microsserviços é difícil, porque eles são separados, com bancos de dados próprios. O que era simples em sistemas monolíticos, aqui vira um problema.

Se você percebe que está precisando de muitas transações entre serviços, talvez eles estejam pequenos demais. Redefinir os limites dos serviços costuma resolver.

Mas sim, em alguns casos, é inevitável fazer transações entre serviços. Aí entram os padrões de compensação, como:

Padrão Saga

Um mediador organiza os passos.

Cada passo é registrado.

Se tudo der certo, beleza.

Se algo falhar, ele desfaz tudo o que foi feito antes (compensação).

Isso gera muita complexidade e tráfego de rede.

Outra opção é implementar ações de “fazer e desfazer” (do/undo) para cada etapa. Isso exige mais esforço na hora de programar e manter, mas reduz a dependência em tempo real.

Mesmo sendo possível fazer transações em microsserviços, isso vai contra o espírito do estilo. Mas, em casos especiais, pode ser necessário.

Conclusão
A arquitetura de microsserviços oferece:

Alta escalabilidade

Facilidade para evoluir

Boa para empresas que mudam rápido

Mas tem seus desafios:

Desempenho pode sofrer por causa das chamadas de rede

Segurança precisa ser bem pensada

Técnicas como cache, coreografia e um bom design ajudam a minimizar os problemas.

Lembrete final: Microsserviço é só o nome, não quer dizer que o serviço tem que ser pequeno de verdade.


