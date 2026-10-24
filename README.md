#  PROJETO — SISTEMA BANCÁRIO EM PYTHON

##  Tema do Projeto
### Simulação de Operações e Fluxos Bancários via Linha de Comando (CLI)

---

##  Sobre o Projeto

Este projeto consiste no desenvolvimento de um **Sistema Bancário Simulado**, construído inteiramente na linguagem **Python**. A aplicação reproduz as regras de negócio e as operações fundamentais presentes no cotidiano de uma instituição financeira tradicional, rodando diretamente via linha de comando.

O foco central do projeto foi o design de software com foco em **validação rígida de dados**, controle de fluxos de estado (manutenção de saldo), segurança de acesso e tratamento de possíveis inconsistências causadas por entradas incorretas do usuário.

---

##  Funcionalidades do Sistema

O sistema simula uma esteira de autoatendimento bancário estruturada em camadas:

*  **Módulo de Autenticação:** Camada inicial de segurança simulada exigindo a validação dos últimos dígitos do cartão, CPF e senha de acesso.
*  **Depósitos:** Entrada de valores monetários com atualização automática e cumulativa do saldo da conta.
*  **Saques:** Retirada de fundos parametrizada por travas de segurança (verificação de saldo disponível e limite de fundos).
*  **Consulta de Dados:** Visualização estruturada das informações cadastrais do cartão do cliente.
*  **Encerramento Seguro:** Finalização correta dos loops de execução da aplicação.

---

##  Conceitos e Lógica Aplicada

* **Controle de Fluxo e Menu:** Uso de laços iterativos infinitos controlados (`while`) para manter o menu ativo até a ação explícita de saída.
* **Tomadas de Decisão Complexas:** Estruturas condicionais encadeadas (`if/elif/else`) mapeando cada regra de negócio e operação escolhida.
* **Sanitização de Inputs:** Lógica para garantir que dados puramente numéricos sejam inseridos em campos de valores, evitando falhas de execução no sistema.

---

##  Demonstração da Interface (CLI)

O sistema interage com o usuário por meio de prompts de texto organizados no terminal da seguinte forma:

```text
=================== SISTEMA BANCÁRIO ===================

[1] Depositar
[2] Sacar
[3] Visualizar Cartão
[4] Sair

Digite a opção desejada: _
```

---

##  Estrutura do Repositório

```text
└── Banco.ipynb                         # Código-fonte principal com a lógica do sistema bancário
```

---

##  Observação Importante

Este software possui caráter **puramente educacional e didático**. Os estados da conta e as informações de login do cliente são processados e mantidos em memória volátil durante a execução do script, não possuindo integrações com bancos de dados relacionais reais ou APIs de pagamentos de terceiros.

---

##  Referência

Projeto prático desenvolvido para consolidação de algoritmos de manipulação de tipos primitivos, variáveis locais e lógica de programação em ambientes imperativos.
