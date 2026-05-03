# dados-atletas
O objetivo deste projeto é aplicar conceitos de Programação Orientada a Objetos (POO) em JavaScript para gerenciar dados de atletas. O software recebe informações básicas (nome, idade, peso, altura e notas), processa esses dados através de métodos específicos e retorna resultados cruciais para organizadores de competições, como a categoria por idade, o IMC e a performance técnica (média de notas).

A Lógica de Negócio
O sistema não apenas armazena dados, mas aplica regras automáticas:
Categorização: Define o grupo do atleta com base na idade.
Saúde: Calcula o Índice de Massa Corporal (IMC).
Performance: Calcula uma média "justa", eliminando os extremos (a maior e a menor nota), garantindo que a pontuação reflita a constância do atleta.

Estrutura da Classe Atleta
A classe funciona como um molde. Cada vez que você cria um "novo atleta", ele carrega os seguintes componentes:
1. Atributos (Dados)
nome, idade, peso, altura e notas (um array de números).

2. Métodos de Cálculo (Processamento)
calculaCategoria(): Usa estruturas condicionais (if/else) para retornar a faixa etária.
calculaIMC(): Aplica a fórmula física $IMC = \frac{peso}{altura^2}$.
calculaMediaValida(): Ordena as notas, descarta a menor e a maior, e tira a média das três restantes.

3. Métodos de Retorno (Saída)
Funções iniciadas com obtem... que servem para expor os resultados processados para o usuário final.

Como Executar o Projeto
Para rodar este código, você não precisa instalar ferramentas complexas. Siga um dos métodos abaixo:

Opção A: Navegador (O mais rápido)
Abra qualquer navegador (Chrome, Edge, Firefox).
Pressione F12 (ou clique com o botão direito e selecione Inspecionar).
Vá na aba Console.
Cole o código da classe e o exemplo de uso.
Pressione Enter.

Opção B: Node.js (Localmente)
Crie um arquivo chamado atleta.js.
Cole o código dentro dele.
Abra o terminal na pasta do arquivo.
Digite o comando: node atleta.js.

Exemplo de Fluxo de Dados
Ao instanciar a classe com o exemplo fornecido:
Entrada: 30 anos, 80kg, 1.70m, notas [10, 9.34, 8.42, 10, 7.88]
Processamento da Média:
Ordena: [7.88, 8.42, 9.34, 10, 10]
Remove extremos: [8.42, 9.34, 10]
Média: (8.42+9.34+10)/3=9.2533...
Saída: O objeto retorna todos os dados formatados conforme as especificações.





