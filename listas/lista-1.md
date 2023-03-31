 *Obs.: Neste momento, evite usar funções existentes para resolução das questões*

# Questões

> Será utilizado Python para a resolução dos exercícios

1. Escreva uma função chamada multiplica que faça multiplicação de dois números inteiros utilizando somas.

    ```python
    def multiplica(a, b):
        if (b == 0): return a
        return a + multiplica(a, b-1)
    ```
2. Escreva uma função chamada divide que faça divisão de dois números inteiros utilizando subtrações.
    
    ```python
    def divide(a, b):
        if (b == 0): raise ZeroDivisionError("Cannot divide by zero")
        q = 0
        while (a >= b):
            q += 1
            a -= b
        return q
    ```

3. Escreva uma função chamada potencia que calcule a potência de dois números x e y (xy) utilizando multiplicações.
    
    ```python
    def potencia(x, y):
        if (y == 0): return 1
        return x * potencia(x, y-1)
    ```

4. Escreva uma função chamada primo que recebe um número inteiro e retorne 1, se primo, ou 0, caso contrário.
    
    ```python
    def primo(x):
        if (x <= 1): return 0
        i = 2
        while (i*i <= x):
            if (x%i == 0): return 0
            i += 1
        return 1
    ```

5. Escreva uma função chamada fatorial que recebe um número e retorne seu fatorial.
    
    ```python
    def fatorial(x):
        if (x == 0): return 1
        return x * fatorial(x-1)
    ```
    
6. Escreva uma função chamada inteiros que recebe um número inteiro positivo x e retorne a soma de todos os inteiros positivos entre 1 e x.
    
    ```python
    def inteiros(x):
        return x*(x+1)/2
    ```
    
7. Escreva uma função chamada fibonacci que receba um número e retorne a soma da sua sequência de Fibonacci.
    
    ```python
    def fibonacci(x):
        sum = 0
        last = 0
        curr = 1
        for i in range(x):
            sum += curr
            last, curr = curr, last + curr
        return sum
    ```
    
8. Se listarmos todos os números naturais abaixo de 10 que são múltiplos de 3 ou 5, temos 3, 5, 6, 9, cuja soma é 23. Escreva uma função chamada multiplos que recebe um número y e retorna a soma de todos os múltiplos de 3 e 5 abaixo desse número y.
    
    ```python
    ```
    
9. Escreva uma função chamada maior que recebe um vetor e retorna o maior valor dentre os elementos do vetor.
    
    ```python
    ```
    
10. Escreva uma função chamada menor que recebe um vetor e retorna o maior valor dentre os elementos do vetor.
    
    ```python
    ```
    
11. Escreva uma função chamada media que recebe um vetor e retorna sua média.
    
    ```python
    ```
    
12. Escreva uma função chamada somamatriz que recebe uma matriz e soma todos os elementos da matriz.
    
    ```python
    ```
    
13. Escreva uma função chamada somacoluna que recebe uma matriz, calcula sua transposta e soma os elementos da primeira coluna.
    
    ```python
    ```
    
14. Escreva uma função chamada somadiagonal que recebe uma matriz e calcula a soma dos elementos que estão na diagonal principal.
    
    ```python
    ```
    
15. Escreva uma função chamada pertence que recebe dois vetores e retorna a soma dos elementos que fazem parte dos dois conjuntos (vetores).
    
    ```python
    ```
