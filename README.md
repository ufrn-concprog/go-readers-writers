# Trabalho Prático: O Problema dos Leitores e Escritores (Go Version)

<sub>Última atualização: 21/11/2025</sub>

## Sumário

- [Objetivo](#objetivo)
- [Introdução](#introdução)
- [Tarefas](#tarefas)
  - [Implementação](#implementação)
  - [Relato](#relato)
- [Autoria e política de colaboração](#autoria-e-política-de-colaboração)
- [Entrega](#entrega)
- [Avaliação](#avaliação)
- [Dúvidas e informações](#dúvidas-e-informações)

## Objetivo

O objetivo deste trabalho é estimular o projeto e a implementação de soluções para problemas por meio de programação concorrente, mais especificamente, utilizando a linguagem de programação [Go](https://go.dev).

## Introdução

O Problema dos Leitores e Escritores (*Readers-Writers Problem*) é um problema clássico no contexto de programas concorrentes, que serve, inclusive, como modelo para outros problemas com características semelhantes. Proposto originalmente por P. J. Courtois, F. Heymans e D. L. Parnas em seu artigo [*Concurrent control with "readers" and "writers"*](https://doi.org/10.1145/362759.362813), publicado em 1971, o problema diz respeito à existência de um recurso compartilhado entre dois tipos de processos (leitores e escritores) que tentam acessá-lo simultaneamente. Os processos leitores realizam operações de leitura sobre o recurso compartilhado, enquanto os processos escritores realizam operações de escrita. O problema consiste, portanto, em estabelecer uma forma de sincronização entre esses processos de modo a preservar um estado consistente do recurso compartilhado.

## Tarefas

A tarefa central a ser realizada neste trabalho consiste em produzir uma nova versão das soluções implementadas para o Problema dos Leitores e Escritores (ver o trabalho original [aqui](https://github.com/ufrn-concprog/readers-writers/)), desta vez utilizando os recursos da linguagem de programação Go. Deverá ser implementada tanto uma versão que dá preferência aos leitores quanto a que dá preferência aos escritores, bem como, para fins de demonstração, um código-fonte principal que instancie um determinado número de gorotinas para realizar operações de leitura e escrita sobre alguma variável, objeto ou arquivo (recurso compartilhado). A execução do programa deverá exibir, na saída padrão, o comportamento das gorotinas no tocante ao acesso ao recurso compartilhado e a eventuais bloqueios caso o recurso compartilhado esteja em uso.

### Relato

Uma vez realizadas as tarefas de implementação, deverá ser elaborado um relatório sucinto, pelo menos, uma descrição acerca:

- de como a solução foi projetada;
- um comparativo, quanto a esforço de programação, com relação ao programa anteriormente desenvolvido;
- eventuais dificuldades encontradas durante o desenvolvimento, e;
- instruções para a compilação e a execução do programa.

## Autoria e política de colaboração

Este trabalho deverá ser realizado em equipe composta por até dois estudantes, sendo importante, dentro do possível, dividir as tarefas de forma igual entre os integrantes. Após a implementação das soluções para os problemas propostos, o arquivo [`author.md`](https://github.com/ufrn-concprog/go-readers-writers/tree/master/author.md) presente no repositório deverá ser editado, preenchendo as informações de identificação dos integrantes da equipe na seção [Informações de Autoria](https://github.com/ufrn-concprog/go-readers-writer/tree/master/author.md#identificação-de-autoria).

O trabalho em cooperação entre estudantes da turma é estimulado, sendo admissível a discussão de ideias e estratégias. Contudo, tal interação não deve ser entendida como permissão para utilização de (parte de) código-fonte de colegas, o que pode caracterizar situação de plágio. **Trabalhos copiados, no todo ou em parte, de outros colegas ou da Internet, ou ainda gerados por ferramentas de Inteligência Artificial serão anulados e receberão nota zero.**

## Entrega

O sistema de controle de versões [Git](https://git-scm.com) e o serviço de hospedagem de repositórios [GitHub](https://github.com) serão utilizados para viabilizar a entrega da implementação. Para possibilitar a associação de repositórios do Git a cada equipe e reuni-los em uma mesma infraestrutura, foi criada uma atividade (*assignment*) no GitHub Classroom. Cada integrante da equipe deverá acessar o GitHub Classroom pelo *link* fornecido e, em seguida, seguir as instruções na tela para acessar a atividade e, se necessário, criar uma equipe. Este [vídeo](https://youtu.be/ObaFRGp_Eko) demonstra como ocorre esse processo.

Ao criar uma equipe, o GitHub Classroom cria um repositório Git privado, acessível apenas aos integrantes da equipe e ao docente, na organização [`ufrn-concprog`](https://github.com/ufrn-concprog). A fim de garantir a boa manutenção do repositório, deve-se ainda configurar corretamente o arquivo `.gitignore` para desconsiderar arquivos que não devem ser versionados, como os executáveis gerados na compilação do código-fonte.

A entrega deste trabalho deverá ser realizada até as **23:59 do dia 13 de dezembro de 2025** no respectivo repositório Git da equipe. O relatório elaborado, preferencialmente em formato *Adobe Portable Format* (PDF), deverá ser enviado como arquivo através da opção *Tarefas* da Turma Virtual do SIGAA, juntamente com, no campo *Comentários*, o endereço do repositório. Um único membro da equipe deve realizar esse envio e não serão aceitos envios por outros meios ou repositórios que não sejam os descritos nesta especificação.

## Avaliação

A avaliação do trabalho contabilizará nota máxima de 10,0 pontos na 3ª Unidade da disciplina. O trabalho será avaliado de acordo com os seguintes critérios:

- utilização correta das facilidades de programação concorrente em Go;
- a corretude da execução do programa implementado, tanto com relação a funcionalidades quanto à concorrência;
- a aplicação de boas práticas de programação, incluindo legibilidade, organização e documentação de código-fonte;
- correta utilização do repositório Git, no qual deverá ser registrado todo o histórico da implementação por meio de *commits*, e;
- qualidade do relatório produzido

## Dúvidas e informações

Caso haja qualquer dúvida, questionamento ou necessidade de informação adicional, é possível:

- enviar *e-mail* para o endereço <everton.cavalcante@ufrn.br>;
- enviar mensagem privada diretamente ao docente, utilizando o servidor Discord;
- enviar mensagem no canal de texto `#duvidas` no servidor Discord, ou;
- agendar encontros síncronos pelo canal de áudio `Fale com Prof. Everton` no Discord.
