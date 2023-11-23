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

  Questões de Teste:

  C++ Features Overview

ChatGPT 3.5

Faça um resumo do que é a linguagem de reprogramação C++. Destaque separadamente tudo que for mais relevante e que possa cair em uma prova da faculdade.

ChatGPT
A linguagem de programação C++ é uma extensão da linguagem C, incorporando programação orientada a objetos e oferecendo recursos como:

Orientação a Objetos: Suporte a conceitos como classes e herança, permitindo a organização de código de forma modular e reutilizável.

Polimorfismo: Possibilidade de criar funções com o mesmo nome, mas com comportamentos diferentes, facilitando a manipulação de diferentes tipos de dados.

Encapsulamento: Capacidade de esconder a implementação interna de uma classe e fornecer uma interface clara para interação.

Templates: Mecanismo que permite criar funções e classes genéricas, permitindo a criação de algoritmos e estruturas de dados flexíveis.

Gerenciamento de Memória: Combinação de alocação automática e alocação dinâmica de memória, com suporte a ponteiros.

Sobrecarga de Operadores: Habilidade de definir comportamentos específicos para operadores, adaptando-os para tipos de dados personalizados.

Manipulação de Exceções: Introduz mecanismos para lidar com erros de forma estruturada, melhorando a robustez do código.

Esses aspectos são essenciais para compreender a fundo a C++ e são frequentemente abordados em provas de programação em nível acadêmico.




Agora simule questões de uma prova real de liguagem C++

ChatGPT
Questão 1:
Explique a diferença entre uma classe abstrata e uma classe concreta em C++. Dê um exemplo prático de quando seria apropriado usar cada uma.

Questão 2:
Como o polimorfismo é implementado em C++? Forneça um exemplo de código que demonstre o uso de polimorfismo com classes e funções virtuais.

Questão 3:
Explique o que é uma exceção em C++. Como você pode lidar com exceções usando blocos try-catch? Dê um exemplo de código.

Questão 4:
O que são templates em C++ e qual é o propósito de usá-los? Forneça um exemplo de uma função ou classe que utiliza templates.

Questão 5:
Como funcionam os ponteiros em C++? Explique a diferença entre ponteiros e referências, dando exemplos de situações em que cada um seria mais apropriado.

Questão 6:
Descreva o que é o operador de sobrecarga em C++. Dê um exemplo de como você poderia sobrecarregar o operador de adição para duas classes personalizadas.

Questão 7:
Qual é a diferença entre a alocação de memória estática e dinâmica em C++? Quando seria apropriado usar uma em vez da outra? Dê exemplos práticos.

Lembre-se de que as respostas devem ser claras, concisas e demonstrar um entendimento sólido dos conceitos mencionados.

RESPOSTAS:

Resposta 1:
Uma classe abstrata em C++ é uma classe que contém pelo menos uma função virtual pura, tornando-a incompleta e impossível de ser instanciada. Uma classe concreta, por outro lado, é completamente implementada e pode ser instanciada. Um exemplo de uso apropriado de uma classe abstrata seria definir uma classe base para formas geométricas, enquanto uma classe concreta seria uma implementação específica, como uma classe "Círculo".

Resposta 2:
O polimorfismo em C++ é alcançado por meio de funções virtuais e ponteiros para objetos da classe base. Exemplo:


class Animal {
public:
    virtual void fazerSom() {
        // implementação padrão
    }
};

class Cachorro : public Animal {
public:
    void fazerSom() override {
        std::cout << "Au Au!" << std::endl;
    }
};
Resposta 3:
Uma exceção em C++ é um mecanismo para lidar com erros durante a execução do programa. Blocos try-catch são usados para capturar e tratar exceções. Exemplo:


try {
    // Código que pode gerar uma exceção
    throw std::runtime_error("Ocorreu um erro!");
}
catch (const std::exception& e) {
    std::cerr << "Exceção capturada: " << e.what() << std::endl;
}
Resposta 4:
Templates em C++ são modelos que permitem a criação de funções e classes genéricas. Exemplo de uma função de troca usando templates:


template <typename T>
void trocar(T& a, T& b) {
    T temp = a;
    a = b;
    b = temp;
}
Resposta 5:
Ponteiros em C++ são variáveis que armazenam endereços de memória. A diferença entre ponteiros e referências é que ponteiros podem ser reatribuídos, enquanto referências são aliases imutáveis. Exemplo:


int valor = 42;
int* ponteiro = &valor;
int& referencia = valor;
Resposta 6:
A sobrecarga de operadores em C++ permite definir comportamentos personalizados para operadores. Exemplo de sobrecarga do operador de adição para duas classes:


class Complexo {
public:
    int real;
    int imaginario;

    Complexo operator+(const Complexo& outro) {
        Complexo resultado;
        resultado.real = real + outro.real;
        resultado.imaginario = imaginario + outro.imaginario;
        return resultado;
    }
};
Resposta 7:
A alocação de memória estática ocorre em tempo de compilação, enquanto a alocação dinâmica ocorre em tempo de execução usando new e delete. Use alocação estática para objetos de tamanho fixo conhecido antecipadamente e alocação dinâmica para objetos de tamanho desconhecido ou que precisam persistir além do escopo atual. Exemplos:


// Alocação estática
int arrayEstatico[5];

// Alocação dinâmica
int* arrayDinamico = new int[5];
delete[] arrayDinamico;
