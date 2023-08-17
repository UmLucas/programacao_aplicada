# Disciplina de Programação Aplicada
Repositório da disciplina de Programação Aplicada.

## Aula 1: Introdução da Disciplina
Texto referente ao resumo da aula 1.

## Aula 2: Linguagem C (Parte 1)
1. Introdução ao Python e a linguagem C
Texto referente a home e intro das linguagens.
2. Comparação entre Python e C
Como funciona a linguagem python e C em detales (vai cair na prova)
Como executar um bloco de notas no cmd
3. Syntaxe do Python e C
A syntaxe do Python pode ser executada escrevendo direto no cmd
Ou criando um arquivo python no servidor, usando a extenção de arquivo .py e rodando no cmd
- Python:
  - Indentação refere-se aos espaços no início das linhas do código (Mais precisamente quando pressionamos TAB);
  - Enquanto em outras linguagens a indentação serve apenas para deixar mais legível, no python ela é muito importante, pois ela liga linhas de código nos mesmo espaços.
- C:
  - A indentação não serve pra nada, não é necessário deixar esses espaços, já que espaços não são lidos em C;
  - Para compilar um código é necessário utilizar os seguintes comandos:

        int main()
        {
        return 0;
        }
  - Para mostrar o resultado dos códigos é necessário adicionar a biblioteca stdio.h:

        #include <stdio.h>
    
        int main()
        {
          printf("Olá meu nobre!");
          return 0;
        }
4. Output
- Python:
  
              s = "seg"
              t = "terça"
              q = "quarta"
              bd1 = "BD1"
              f1 = "Física 1"
              c1 = "Cálculo 1"
              print("|{:10}|{:10}|{:7}".format(s, t, q))
              print("--------------------------------")
              print("|{:10}|{:10}|{:10}".format(bd1, f1, c1))
            }
- C:
  
                int main() {
                  printf("| Segunda \t| Terça \t| Quarta \t|\n");
                  printf("---------------------------------\n");
                  printf("| BD1 \t\t| Física 1 \t| Cálculo 1 \t|\n");
                  return 0;
                }
  
5. Comentários
6. Variáveis
  - Tipos primitivos:
    - int
    - float
    - char
  - Obs:
    Em python eu declaro classes e não variáveis.

## Aula 3:
- Saída de dados em C: printf();
- Entrada de dados em C: sacanf();
  - é necessário acrescentar "%i" e "&variável", quando quero imprimir um número;
  - para imprimir um nome é necessário usar char variavel[numero];
- Exemplo 1:
  
          int main(void) {
          char nome;
          int idade;
          
          //A função printf é de saída de dados
          //A funçao sancf é de entrada de dados
          printf("Hello World\n"); //Função de saída de dados. \n adiciona uma nova linha
          printf("Iniciando a aprendizagem da linguagem C\n");
          
          //printf("Digite seu nome: \n");
          //scanf("%s", nome); //Como se fosse o input() da linguagem python
          //printf("Seja bem-vindo, %s", nome);
        
          printf("Digite a sua idade: ");
          scanf("%i", &idade);
          printf("Sua idade  é: %i", idade);
          return 0;
        }
