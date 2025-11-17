## 📦 Order Register CLI (Java)

Este é um projeto de uma aplicação **CLI (Command Line Interface)** desenvolvida em **Java** para gerenciar um registro básico de pedidos. O sistema permite cadastrar dados de um cliente e associar a ele uma quantidade variável de pedidos, cada um com um status definido por tipos `enum`.

---

## ✨ Funcionalidades

O CLI é focado na manipulação de entidades Cliente e Pedido, garantindo a integridade dos dados através do uso de tipos enumerados para o status.

* **Cadastro de Clientes:** Permite registrar os dados essenciais de um novo cliente.
* **Cadastro de Pedidos (N por Cliente):** Permite adicionar múltiplos pedidos a um cliente existente.
* **Controle de Status:** Cada pedido é marcado com um status que utiliza tipos `enum` (por exemplo: PENDENTE, PROCESSANDO, ENVIADO, ENTREGUE).
* **Estrutura de Dados:** Demonstra o uso de coleções e a relação "um-para-muitos" (um cliente para N pedidos).

---

## 🛠️ Tecnologias Utilizadas

Este projeto foi desenvolvido utilizando puramente a linguagem:

* **Java** (versão 8 ou superior)

---

## 🚀 Como Executar

### Pré-requisitos

Certifique-se de ter o **Java Development Kit (JDK)** instalado em sua máquina.

### Compilação e Execução

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/vncssd/Order.git]
    cd [pasta-do-projeto]
    ```

2.  **Compile os arquivos Java:**
    Se o seu arquivo principal for `OrderRegisterCLI.java` e estiver no diretório `src/`:
    ```bash
    javac src/*.java
    ```

3.  **Execute o programa:**
    Assumindo que sua classe principal se chama `OrderRegisterCLI`:
    ```bash
    java -cp src OrderRegisterCLI
    ```
    *Obs: Os comandos exatos podem variar dependendo da estrutura de pastas e do nome da sua classe principal.*

---

## 📝 Detalhes da Implementação (Exemplo)

O coração do projeto reside nas classes e na enumeração de status:

### Exemplo de `StatusPedido.java`
```java
public enum StatusPedido {
    PENDENTE,
    PROCESSANDO,
    ENVIADO,
    ENTREGUE,
    CANCELADO
}
