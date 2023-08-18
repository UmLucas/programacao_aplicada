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
- Exemplo 2:
  
      /*
      Média do Aluno
      */
      
      #include <stdio.h>
      
      int main(void)
      {
        int n1, suc, ant;
      
        printf("Digite a primeira nota do aluno: \n");
        scanf("%f", &n1);
        suc = n1 - 1;
        ant = n1 + 1;
        printf("O antecessor do seu némero é: %i\n", &ant);
        printf("O sucessor do seu número é: %i\n", &suc);
        return 0;
      }

- Exemplo 3:
  

- A liguagem C possui 4 tipos de dados primitios.
  - Cada um armazena um tipo de informação possui um tamanho diferemte em bytes.
  
    - char   1 byte  Armazena caraceres.
    - int    4 bytes Armazena números inteiros.
    - float  4 bytes Armazena números reais até 6 casas decimais.
    - double 8 bytes Armazena números reais até 15 casas decimais.
- Exemplo 4:

        char minhaLetra = 'R';
        int copaDoBrasil = 1991;
        float floatPi = 3.1415;
        double doublePi = 3.1415;
        printf("Caracter: \t\t%c. \t\t\tTamanho: %lucas byte(s).\n", minhaLetra, sizeof(minhaLetra));
        printf("Valor int: \t\t%i. \t\tTamanho: %lucas byte(s).\n", copaDoBrasil, sizeof(copaDoBrasil));
        printf("Valor float: \t%f. \tTamanho: %lucas byte(s).\n", floatPi, sizeof(floatPi));
        printf("Valor double: \t%f. \tTamanho: %lucas byte(s).\n", doublePi, sizeof(doublePi));
        
        return 0;
      }
2. Modificadores de Tipos de Dados
- A linguagem C possui 4 tipos de modificadores de tipo.
- Estes modificadores definem um novo tamanho ou sinal para as variáveis.

    - short     Divide pela metade o tamanho d uma variável.
    - long      Dobra o tamanho de uma variável.
    - signed    Define como números apenas positivos.
    - unsigned  Define como números positivos e negaivos.
- Exemplo:

      signed int x = 200;
      unsigned int y = -100;
    
      printf()
      return 0;
    }
