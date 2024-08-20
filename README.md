## Getting Started

Welcome to the VS Code Java world. Here is a guideline to help you get started to write Java code in Visual Studio Code.

## Folder Structure

The workspace contains two folders by default, where:

- `src`: the folder to maintain sources
- `lib`: the folder to maintain dependencies

Meanwhile, the compiled output files will be generated in the `bin` folder by default.

> If you want to customize the folder structure, open `.vscode/settings.json` and update the related settings there.

## Dependency Management

The `JAVA PROJECTS` view allows you to manage your dependencies. More details can be found [here](https://github.com/microsoft/vscode-java-dependency#manage-dependencies).

Projeto: Processo Seletivo
Este projeto simula um processo seletivo simplificado, onde diferentes candidatos são avaliados com base em seus salários pretendidos, e tentativas de contato são realizadas para confirmar a aceitação dos candidatos. O projeto está implementado em Java e utiliza estruturas de controle de fluxo como loops e condicionais para gerenciar as operações.

Funcionalidades
O código possui as seguintes funcionalidades:

Contato com Candidatos:

Método: entrandoEmContato(String candidato)
Descrição: Realiza até três tentativas de contato com um candidato. Se o contato for bem-sucedido dentro das três tentativas, exibe uma mensagem de sucesso; caso contrário, exibe uma mensagem de falha.
Lógica: Utiliza um loop do-while para tentar o contato. O resultado da tentativa é determinado aleatoriamente pela função atender().
Impressão de Candidatos Selecionados:

Método: imprimirSelecionados()
Descrição: Imprime a lista de candidatos com o índice de cada um. Também utiliza um loop for-each para iterar sobre os candidatos e exibir seus nomes.
Lógica: O método exibe os candidatos de duas maneiras: com índice explícito e com a forma abreviada de for-each.
Seleção de Candidatos Baseada em Salário Pretendido:

Método: selecaoCandidatos()
Descrição: Seleciona até cinco candidatos que têm uma pretensão salarial menor ou igual ao salário base disponível (2000.0).
Lógica: Utiliza um loop while para iterar sobre os candidatos e, para cada um, gera um salário pretendido aleatório entre 1800.0 e 2200.0 através do método valorPretendido().
Análise de Candidato com Base no Salário Pretendido:

Método: analisarCandidato(double salariopretendido)
Descrição: Avalia o candidato com base no salário pretendido e o compara com o salário base (2000.0). Dependendo do resultado, diferentes mensagens são impressas.
Lógica: Utiliza condicionais if-else para determinar a ação a ser tomada (contato imediato, contraproposta ou espera).
Estrutura do Projeto
O código está organizado em uma única classe, ProcessoSeletivo, que contém todos os métodos relevantes para a simulação do processo seletivo.

entrandoEmContato(String candidato): Método para tentar contato com o candidato.
imprimirSelecionados(): Método para imprimir a lista de candidatos selecionados.
selecaoCandidatos(): Método para selecionar candidatos com base no salário pretendido.
analisarCandidato(double salariopretendido): Método para analisar o candidato com base no salário pretendido.
valorPretendido(): Método auxiliar que gera um valor aleatório de salário pretendido.
atender(): Método auxiliar que simula a resposta de um candidato ao contato.
Como Executar
Para executar o projeto, basta compilar e rodar a classe principal ProcessoSeletivo. Certifique-se de ter o JDK instalado em sua máquina.

Compilação
bash
Copiar código
javac ProcessoSeletivo.java
Execução
bash
Copiar código
java ProcessoSeletivo
Observações
Este projeto serve como uma prática de estruturas de controle de fluxo em Java, demonstrando como utilizar loops, condicionais, e geração de valores aleatórios para simular um cenário do mundo real em um processo seletivo.
