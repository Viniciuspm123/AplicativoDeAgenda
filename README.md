## Projeto - Agenda de Contatos (Java Swing)

Este projeto implementa um **aplicativo de agenda simples** com interface gráfica de usuário (GUI) em Java, utilizando a biblioteca **Swing**. O objetivo é permitir que o usuário adicione e visualize uma lista de contatos (nome, telefone, e-mail).

### 🚀 Sobre o Projeto

O aplicativo `AgendaSwing` possui uma interface dividida em três áreas principais: um formulário para entrada de dados (Nome, Telefone, Email), uma área para botões (`Adicionar` e `Limpar`), e uma área de texto para exibir a lista completa de contatos cadastrados. Todos os contatos são armazenados em uma `ArrayList` enquanto o aplicativo está em execução.

### 🛠️ Tecnologias e Conceitos Abordados

**Java Swing e GUI:**
Criação da janela principal estendendo (JFrame) e uso de componentes como (JTextField) para entrada, (JTextArea) para exibição e (JButton) para ações.

**Layouts:**
Utilização do gerenciador de layout `(BorderLayout)` para organizar as principais seções da janela (Formulário, Botões, Lista de Contatos).
Uso do `(GridLayout)` para organizar os rótulos e campos de texto do formulário em uma estrutura $4 \times 2$.
Uso do `(FlowLayout)` para centralizar os botões de ação.

**Estrutura de Dados:**
A classe `(Contato)` é usada para modelar a informação de cada contato (Nome, Telefone, Email).
A estrutura `(ArrayList)` é usada para armazenar e gerenciar a coleção de objetos `Contato` na memória.

**Gerenciamento de Eventos e Ações:**
Implementação da interface `(ActionListener)` nos botões `Adicionar` e `Limpar`.
O método `actionPerformed` é responsável por:
1.  **Adicionar Contato:** Captura os textos dos campos, cria um novo objeto `Contato`, adiciona-o à lista, atualiza a exibição (`atualizarListaContatos`) e limpa os campos.
2.  **Limpar Campos:** Reseta os campos de entrada e foca no campo Nome.

**Exibição de Dados:**
O método `atualizarListaContatos` itera sobre a `ArrayList` e constrói a string de exibição no `(JTextArea)`, utilizando o método `toString()` da classe `Contato`.

**Event Dispatch Thread (EDT):**
O método `main` garante que a aplicação seja iniciada corretamente na thread de eventos do Swing.

### 💻 Como Executar

Clone este repositório.

Este projeto deve ser compilado e executado através de um ambiente de desenvolvimento Java (IDE), como Eclipse ou IntelliJ, ou via terminal.
