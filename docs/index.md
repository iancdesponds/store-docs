# Documentação — Projeto em Grupo de Plataformas, Microsserviços e APIs

Trabalho desenvolvido por **Ian Desponds** e **Beni Sliozbergas** na disciplina *Plataformas, Microsserviços e APIs* (Turma 25.1) – Ciência da Computação, Insper.

---

## Visão Geral

O ecossistema é composto por dez microsserviços principais — cada um versionado em um repositório separado — além de um serviço auxiliar de *benchmark* (Bottleneck). O objetivo do projeto foi:

* **Modelar** uma arquitetura de microsserviços completa (contas, autenticação, catálogo, pedidos, etc.).
* **Implementar** APIs REST com Java + Spring Boot.
* **Automatizar** integração e entrega contínuas (CI/CD) e orquestração em Kubernetes.
* **Garantir** observabilidade, escalabilidade horizontal e boas práticas de segurança.

---

## Repositórios

| Domínio                | Interface                                                                                      | Service (implementação)                                                                                        |
| ---------------------- | ---------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- |
| **Account**            | [microservicos-account](https://github.com/Benibergas/microservicos-account){target="\_blank"} | [microservicos-account-service](https://github.com/Benibergas/microservicos-account-service){target="\_blank"} |
| **Auth**               | [microservicos-auth](https://github.com/Benibergas/microservicos-auth){target="\_blank"}       | [microservicos-auth-service](https://github.com/Benibergas/microservicos-auth-service){target="\_blank"}       |
| **Gateway**            | —                                                                                              | [microservicos-gateway-service](https://github.com/Benibergas/microservicos-gateway-service){target="\_blank"} |
| **Exchange**           | —                                                                                              | [microservicos-exchange](https://github.com/Benibergas/microservicos-exchange){target="\_blank"}               |
| **Product**            | [microservicos-product](https://github.com/Benibergas/microservicos-product){target="\_blank"} | [microservicos-product-service](https://github.com/Benibergas/microservicos-product-service){target="\_blank"} |
| **Order**              | [microservicos-order](https://github.com/Benibergas/microservicos-order){target="\_blank"}     | [microservicos-order-service](https://github.com/Benibergas/microservicos-order-service){target="\_blank"}     |
| **Bottleneck Cache** | —                                                                                              | [microservicos-bottleneck](https://github.com/Benibergas/microservicos-bottleneck){target="\_blank"}           |
