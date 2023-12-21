# Aprendendo Ensinando

## Como rodar a aplicação com Docker

### Pré-requisitos

Antes de começar, certifique-se de que você tem o Docker e o Docker Compose instalados em sua máquina.

### Configuração

1. Crie um arquivo `.env` na raiz do projeto (mesmas pasta que fica o pom.xml).

2. Defina as seguintes variáveis no arquivo `.env`:

- `DB_PASSWORD`
- `DB_TEST_PASSWORD`
- `DB_USER`
- `DB_TEST_USER`

Adicione os valores correspondentes a cada uma dessas variáveis.

### Execução

1. Execute o seguinte comando para construir o projeto:

    `mvn clean package -DskipTests`

2. Em seguida, construa a imagem Docker com o seguinte comando:

   `docker-compose build`

3. Finalmente, inicie a aplicação com o seguinte comando:

   `docker-compose up`

Agora, sua aplicação deve estar rodando em um contêiner Docker.