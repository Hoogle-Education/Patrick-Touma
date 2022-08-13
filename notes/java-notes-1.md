# Programação Orientada Objetos

# Classe e Objeto

`Classe` é um molde que nos ajuda a modelar problemas reais.

Criando o joao sem POO:
```java
String nomeJoao;
int idadeJoao;
float alturaJoao;
double quantiaJoao;
```

## Criando classes em java

```java
class Pessoa {

  String nome;
  int idade;
  double altura;
  double quantia;
  double media;

  double somar(double a, double b) {
    return a + b;
  }

  double calculaMedia(double a, double b) {
    media = (a+b)/2.0;
    return media;
  }
}

public class Program {

  public static void main(String[] args) {

    Pessoa joao = new Pessoa();
    Pessoa maria = new Pessoa();

    joao.nome = "Joao da Silva";
    joao.idade = 15;
    joao.altura = 1.70;
    joao.quantia = 100.0;

    joao.calculaMedia(10, 8);
    
    maria.nome = "Maria da Silva";
    maria.idade = 15;
    maria.altura = 1.70;
    maria.quantia = 100.0;

    Pessoa aux = joao;
    joao = maria;
    maria = aux;

  }

}
```

## Ideia de array

O `array` serviu para criarmos diversas variáveis de um mesmo tipo.

```java
String[] nomes;
int[] idades;
float[] alturas;
double[] quantias;
```

## Como trocar variáveis

```java
int a = 2, b = 3;
int aux = a; // (aux = 2, a = 2, b = 3)
a = b; // (aux = 2, a = 3, b = 3)
b = aux;
```