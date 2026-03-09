# L-gica-em-Java-

Aqui estão os exemplos convertidos para Java. O código inclui fluxos condicionais, estruturas de repetição e tratamento de exceções, culminando em um sistema contador.

# 1. Fluxos Condicionais

Exemplo: Verificação de Números Pares ou Ímpares

```java
public class ParOuImpar {
    public static String verificaParOuImpar(int numero) {
        if (numero % 2 == 0) {
            return numero + " é par.";
        } else {
            return numero + " é ímpar.";
        }
    }

    public static void main(String[] args) {
        System.out.println(verificaParOuImpar(10)); // Saída: 10 é par.
        System.out.println(verificaParOuImpar(7));  // Saída: 7 é ímpar.
    }
}
```

# 2. Estruturas de Repetição

Exemplo: Contagem de Números de 1 a N

```java
public class Contagem {
    public static void contagem(int n) {
        for (int i = 1; i <= n; i++) {
            System.out.println(i);
        }
    }

    public static void main(String[] args) {
        contagem(5); // Saída: 1 2 3 4 5
    }
}
```

# 3. Tratamento de Exceções

Exemplo: Capturando Erros de Entrada

```java
import java.util.Scanner;

public class PedeNumero {
    public static int pedeNumero() {
        Scanner scanner = new Scanner(System.in);
        while (true) {
            try {
                System.out.print("Digite um número: ");
                return Integer.parseInt(scanner.nextLine());
            } catch (NumberFormatException e) {
                System.out.println("Entrada inválida. Por favor, digite um número inteiro.");
            }
        }
    }

    public static void main(String[] args) {
        int numero = pedeNumero();
        System.out.println("Você digitou o número: " + numero);
    }
}
```

# 4. Sistema Contador Completo

```java
import java.util.Scanner;

public class SistemaContador {
    public static String verificaParOuImpar(int numero) {
        if (numero % 2 == 0) {
            return numero + " é par.";
        } else {
            return numero + " é ímpar.";
        }
    }

    public static int pedeNumero() {
        Scanner scanner = new Scanner(System.in);
        while (true) {
            try {
                System.out.print("Digite um número: ");
                return Integer.parseInt(scanner.nextLine());
            } catch (NumberFormatException e) {
                System.out.println("Entrada inválida. Por favor, digite um número inteiro.");
            }
        }
    }

    public static void main(String[] args) {
        int numero = pedeNumero();
        
        for (int i = 1; i <= numero; i++) {
            System.out.println(verificaParOuImpar(i));
        }
    }
}
```

# Resumo

Nos exemplos:
- Verifica se um número é par ou ímpar usando estruturas condicionais.
- Counta de 1 até N com um loop `for`.
- Captura exceções para entradas inválidas ao solicitar um número do usuário.
- Integra tudo em um sistema contador que mostra se cada número é par ou ímpar. 

Você pode compilar e executar essas classes em qualquer ambiente Java!
