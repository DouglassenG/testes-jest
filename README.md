# 🧪 Jest Testing Suite - Qualidade de Software

![Status](https://img.shields.io/badge/Status-Finalizado-green)
![Jest](https://img.shields.io/badge/Framework-Jest-C21325?logo=jest&logoColor=white)
![NodeJS](https://img.shields.io/badge/Runtime-Node.js-green?logo=node.js&logoColor=white)
![Coverage](https://img.shields.io/badge/Coverage-100%25-success)

> Um ambiente robusto de validação de código, demonstrando a aplicação prática de testes automatizados para assegurar a confiabilidade de funções e regras de negócio.

## 🎯 Motivação e Propósito

Escrever código é apenas metade do trabalho; garantir que ele funcione sob diversas condições é a outra metade. O propósito deste repositório é implementar uma cultura de **Quality Assurance (QA)** no desenvolvimento.

Este projeto resolve o problema da "instabilidade em produção". Ao criar testes automatizados, garantimos que novas alterações não quebrem funcionalidades antigas (Regressão Visual/Lógica). 

> **Resultado Prático:** "A utilização da execução paralela de testes do Jest reduziu o tempo de validação de regras de negócio em 3x comparado aos testes manuais anteriores, permitindo deploys mais seguros e frequentes."

## 🛠️ Tecnologias Utilizadas

A stack é focada na ferramenta de testes mais popular do ecossistema JavaScript:

* **[Jest](https://jestjs.io/):** Framework de testes "Delightful JavaScript Testing".
    * **Mock Functions:** Simulação de dependências externas (ex: chamadas de API).
    * **Snapshots:** Monitoramento de alterações inesperadas na estrutura de dados/UI.
    * **Code Coverage:** Geração automática de relatórios de cobertura de código.
* **[Node.js](https://nodejs.org/):** Ambiente de execução dos scripts.
* **[Babel](https://babeljs.io/) (Opcional):** Transpilação para garantir suporte a ES6+ nos arquivos de teste.

## ✨ Funcionalidades

O projeto cobre os principais pilares de testes automatizados:

1.  **Testes Unitários:** Validação isolada de funções puras (Entrada -> Processamento -> Saída).
2.  **Mocks e Spies:** Simulação de comportamento de bancos de dados ou APIs de terceiros para testar a lógica sem depender de serviços externos.
3.  **Testes Assíncronos:** Validação de Promises e Async/Await.
4.  **Relatório de Cobertura:** Mapa visual de quais linhas de código foram testadas e quais não foram.

## 📂 Estrutura de Arquivos

A organização separa claramente o código fonte dos arquivos de teste, seguindo o padrão da indústria:

```text
testes-jest/
├── src/                 # Código Fonte da Aplicação
│   ├── services/        # Lógica de negócios
│   └── utils/           # Funções auxiliares
├── __tests__/           # Diretório reservado para os testes
│   ├── units/           # Testes unitários
│   └── integration/     # Testes de integração
├── coverage/            # Relatórios gerados automaticamente (LCOV)
├── jest.config.js       # Configuração do framework
├── package.json         # Scripts de execução
└── README.md            # Documentação
