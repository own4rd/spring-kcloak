# Projeto Exemplo - Spring + Keycloak

Este é um projeto exemplo de integração entre Spring Boot e Keycloak para autenticação e autorização. O objetivo deste projeto é demonstrar como configurar o Keycloak em uma aplicação Spring Boot para fornecer autenticação baseada em OAuth2 e gerenciamento de usuários.

## Tecnologias Utilizadas

- **Spring Boot**: Framework para desenvolvimento de aplicações Java.
- **Keycloak**: Solução de gerenciamento de identidade e acesso (IAM), que fornece autenticação e autorização.
- **Spring Security**: Framework para garantir a segurança de aplicações Spring.
- **OAuth2**: Protocolo de autorização utilizado pelo Keycloak.

## Funcionalidades

- Autenticação de usuários via Keycloak.
- Proteção de endpoints da aplicação com OAuth2.
- Gestão de usuários e permissões através do Keycloak.

## Pré-requisitos

Antes de rodar o projeto, verifique se você tem os seguintes pré-requisitos instalados:

- Java 11 ou superior
- Maven ou Gradle
- Docker (opcional, caso deseje rodar o Keycloak em contêiner)
  
## Como Rodar o Projeto

### Passo 1: Configurar o Keycloak

Se você não tem o Keycloak instalado, pode rodá-lo facilmente usando Docker. Execute o seguinte comando para levantar uma instância do Keycloak localmente:

```bash
docker run -p 8080:8080 -e KEYCLOAK_ADMIN=admin -e KEYCLOAK_ADMIN_PASSWORD=admin -d jboss/keycloak
