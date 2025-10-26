# DigitalLockCounterSystem

O **Digital Lock Counter System** é um projeto de sistema de trava digital baseado em **circuitos sequenciais**, que utiliza **flip-flops**, **portas lógicas** e **contadores síncronos** para simular um mecanismo de desbloqueio em múltiplos níveis.  
O sistema foi desenvolvido e testado utilizando o **CedarLogic**, um simulador de circuitos digitais.

## 🔐 Visão Geral

O projeto representa um **sistema de trava digital multinível**, onde cada nível deve ser desbloqueado por meio de uma sequência específica de contagem.  
A progressão só ocorre quando o contador atinge a combinação correta, garantindo que cada estágio dependa do anterior — simulando assim um **processo de autenticação hierárquico**.

## ⚙️ Características Principais

- Sistema de **contagem sequencial de dois dígitos** por nível.  
- **Desbloqueio condicional**: o avanço ao próximo nível ocorre apenas quando ambos os dígitos do contador estão corretos.  
- Implementação de **flip-flops JK/D** e **portas lógicas** para controle de estados.  
- **Lógica combinacional** para verificação da sequência correta.  
- **CedarLogic** usado para modelagem, simulação e validação dos circuitos.

## 🧩 Conceitos Envolvidos

- **Máquinas de estados finitos (FSMs)**: modelagem do comportamento do sistema de desbloqueio.  
- **Contadores síncronos**: controle preciso da sequência de estados.  
- **Flip-flops**: armazenamento de estados e controle de transições.  
- **Lógica combinacional**: detecção de padrões corretos de entrada.  
- **Clocking e sincronização**: garantia de transições estáveis entre estados.

## 🧠 Estrutura de Funcionamento

1. O sistema inicia em um estado bloqueado (nível 0).  
2. A cada pulso de clock, o contador de dois dígitos incrementa sua contagem.  
3. Quando ambos os dígitos atingem o valor configurado de desbloqueio, o sistema progride para o próximo nível.  
4. Após o último nível ser atingido, o sistema libera a trava (saída “Unlock”).

## 🧰 Ferramentas Utilizadas

- **CedarLogic** — para modelagem e simulação do circuito.  
- **Logisim** *(opcional)* — pode ser usado para visualização adicional ou extensão do projeto.  
- **Diagramas de tempo** — para análise de sincronização e transições de estado.

## 🚀 Resultados

- Simulação funcional de um sistema de trava digital com múltiplos níveis.  
- Validação da lógica de desbloqueio sequencial.  
- Demonstração prática de conceitos de **design digital**, **sistemas síncronos** e **FSMs**.  

## 📁 Estrutura do Projeto

```
DigitalLockCounterSystem/
│
├── diagrams/              # Diagramas de circuito (CedarLogic, PNGs, etc.)
├── docs/                  # Documentação técnica
├── README.md              # Este arquivo
└── project.clg            # Arquivo de simulação CedarLogic
```

## 🔧 Próximos Passos

- Adicionar documentação visual dos circuitos (diagramas de tempo e FSM).  
- Implementar lógica de reset e trava por tempo.  
- Expandir para três níveis ou mais de desbloqueio.  

## 📄 Licença

Este projeto é de código aberto sob a licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.

---

Autor: [Gabriel Bozelli](https://github.com/gbozelli)  
Engenharia de Telecomunicações — UNESP  
Bolsista FAPESP | Pesquisador em Redes e Sistemas Digitais
