# Pass-In.
O Pass-in é um projeto de sistema de gerenciamento de eventos desenvolvido em Java utilizando o framework Spring durante a NLW Unite da Rocketseat. Esta API oferece funcionalidades para organizadores de eventos criarem e gerenciarem eventos, enquanto os participantes podem se inscrever, visualizar informações relevantes e realizar check-in nos eventos.

## Funcionalidades.

### Para Organizadores:

- **Cadastro de Novos Eventos:** Os organizadores podem cadastrar novos eventos, fornecendo detalhes como título, descrição e número máximo de participantes.
- **Visualização de Dados do Evento:** Os organizadores podem visualizar dados detalhados de um evento específico, incluindo a lista de participantes inscritos.

### Para Participantes:

- **Inscrição em Eventos:** Os participantes podem se inscrever em eventos disponíveis, fornecendo seu nome e endereço de e-mail.
- **Visualização de Crachá de Inscrição:** Os participantes podem visualizar seus crachás de inscrição, contendo informações como nome, e-mail, título do evento e link para realização do check-in.
- **Realização de Check-in:** Os participantes podem realizar o check-in nos eventos para os quais estão inscritos.

## Regras de Negócio

- **Inscrição Única:** Um participante só pode se inscrever em um evento uma única vez.
- **Vagas Disponíveis:** Um participante só pode se inscrever em eventos com vagas disponíveis.
- **Check-in Único:** Um participante só pode realizar o check-in em um evento uma única vez.

## Tecnologias Utilizadas.

- **Linguagem de Programação:** Java 17.
- **Framework:** Spring (Spring Initializr).
- **Gerenciamento de Dependências:** Maven.
- **Banco de Dados:** HyperSql.
- **Ferramentas Adicionais:** Hibernate (JPA), Lombok.

## Estrutura do Projeto.

- **Controllers:** Responsáveis por receber e processar as requisições HTTP.
- **Services:** Contêm a lógica de negócios da aplicação.
- **Repositories:** Responsáveis pela interação com o banco de dados.
- **DTOs (Data Transfer Objects):** Utilizados para transferir dados entre o cliente e o servidor.
- **Models:** Representam as entidades do banco de dados.
- **Exceptions Handling:** Tratamento de exceções personalizado para lidar com erros de forma adequada.

## Endpoints Principais.

- **POST /events:** Cria um novo evento.
![1criarevento](https://github.com/matheus3pires/Pass-In_NLW/assets/87993331/8490681b-6632-44b4-8835-9dcd34c8d91e)

- **GET /events/{eventId}:** Obtém os detalhes de um evento específico.
![2](https://github.com/matheus3pires/Pass-In_NLW/assets/87993331/061cf547-8b2e-47c5-8549-dcbb95b4139b)

- **POST /events/{eventId}/attendees:** Realiza a inscrição de um participante em um evento.
![4](https://github.com/matheus3pires/Pass-In_NLW/assets/87993331/79d20652-b61e-4dae-bdba-7b8d90b25420)

- **GET /events/attendees/{eventId}:** Obtém as informações dos participante em um evento.
![3](https://github.com/matheus3pires/Pass-In_NLW/assets/87993331/dc76ca35-f077-46c4-82a0-1b9a9fad0d4c)
 
- **GET /attendees/{attendeeId}/badge:** Obtém o crachá de inscrição de um participante.
![5](https://github.com/matheus3pires/Pass-In_NLW/assets/87993331/fc36bd7d-5ff5-4a18-b442-07e9978ded24)
  
- **POST /attendees/{attendeeId}/check-in:** Realiza o check-in de um participante em um evento.
![image](https://github.com/matheus3pires/Pass-In_NLW/assets/87993331/de8a102d-05ac-4aa2-8d9b-c1d03e3ee12d)

## Minhas Redes

Fique conectado para mais novidades e atualizações. Não hesite em entrar em contato!

- Linkedin: [linkedin.com/in/matheuspiress](https://www.linkedin.com/in/matheuspiress/)
- e-mail: matheuspiressdev@gmail.com
