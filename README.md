API feita com Spring e Java de destino e pacotes para uma agência de viagens.
# API de Agência de Viagem

Esta é uma API RESTful desenvolvida em Java com Spring Boot para gerenciar destinos de viagem, permitindo cadastro, busca, avaliação e exclusão de destinos.

## Pré-requisitos

- Java 17 ou superior
- Maven 3.8+ (ou use o wrapper `mvnw`)
- Git (opcional, para clonar o repositório)

## Como rodar o projeto

1. **Clone o repositório**
   ```bash
   git clone https://github.com/m23052000/api-de-agencia-de-viagens.git
   cd api-de-agencia-de-viagens
   ```

2. **Compile e execute a aplicação**
   ```bash
   mvn spring-boot:run
   ```
   Ou, se preferir, gere o JAR e execute:
   ```bash
   mvn clean package
   java -jar target/*.jar
   ```

3. **Acesse a API**
   - A aplicação estará disponível em: [http://localhost:8080](http://localhost:8080)

## Endpoints principais

- `GET /destinos` — Lista todos os destinos
- `POST /destinos` — Cadastra um novo destino
- `GET /destinos/{id}` — Detalhes de um destino
- `PUT /destinos/{id}` — Atualiza um destino
- `DELETE /destinos/{id}` — Exclui um destino
- `GET /destinos/buscarPorNome/{nome}` — Busca destinos por nome
- `GET /destinos/buscarPorLocalizacao/{localizacao}` — Busca destinos por localização
- `GET /destinos/{id}/descricao` — Descrição detalhada do destino

## Observações

- O projeto utiliza banco de dados em memória (H2), não sendo necessário configurar nada adicional.
- Para testar os endpoints, utilize ferramentas como Postman, Insomnia ou o próprio navegador para requisições GET.

---

Desenvolvido para o desafio de API de Agência de Viagem.
