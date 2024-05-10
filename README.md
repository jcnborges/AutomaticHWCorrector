# Assistente IA para Correção de Exercícios de Programação

O assistente IA proporciona uma forma automática de corrigir exercícios de programação, pode ser usada por qualquer professor que trabalhe em um Ambiente Virtual de Aprendizagem (AVA) capaz de baixar as respostas dos estudantes em um arquivo único compactado.

# Entrada
O assistente é capaz de ler um arquivo PDF contendo o enunciado dos exercícios de programação e corrigir as respostas dos estudantes, que vem compactadas em um arquivo ZIP.

# Saída
O modelo gera um feedback personalizado para cada exercício feito pelo aluno, atribuindo uma nota de 0 a 10 e calculando a média final obtida.

# Dados de teste
Foram empregados dados reais (descaracterizados) para testar o modelo, você pode baixar os arquivos utilizados no teste:

*   Arquivo PDF contendo o enunciado dos exercícios. [Clique aqui para baixar o arquivo PDF de teste](https://raw.githubusercontent.com/jcnborges/AutomaticHWCorrector/main/teste/Lista%201%20-%20Revis%C3%A3o%20da%20linguagem%20Java.pdf)

*   Arquivo ZIP contendo a resposta de cada estudante. [Clique aqui para baixar o arquivo ZIP de teste](https://raw.githubusercontent.com/jcnborges/AutomaticHWCorrector/main/teste/respostas.zip)

# AI Gemini Systems Instructions

As seguintes instruções foram configuradas para serem aplicadas em todas as avaliações dos alunos:



```
Faça a avaliação como se fosse um professor de engenharia de software.
Use os enunciados do PDF para avaliar o exercício do aluno.
Informe se o exercício do aluno diverge do enunciado do PDF.
Atribua uma nota de 0 a 10 a cada exercício e calcule a média final.
Caso o exercício não tenha sido entregue, atribua a nota zero.
Use o nome do arquivo para inferir qual é o exercício.
Forneça um relatório padronizado:
    ## Nome do aluno: <nome> ##
    ## Exercício: <numero> ##
        * Enunciado PDF:        
        * Avaliação do código:
        * Sugestão de melhoria:
        * Nota:
    ## Média final: ##
    ## Dificuldade do aluno:   
```
