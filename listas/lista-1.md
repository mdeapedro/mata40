*Obs.: Neste momento, evite usar funções existentes para resolução das questões*

# Questões

1. Escreva uma função chamada multiplica que faça multiplicação de dois números inteiros utilizando somas.

    > Em Python:
    ```python
    def multiplica(a, b):
        r = 0
        while (b > 1):
            if (b%2 == 1): r += a
            a += a
            b //= 2
        return a + r
    ```
    > Em C++:
    ```c++
    int multiplica(int a, int b) {
        int r = 0;
        while (b > 1) {
            if (b&1) r += a;
            a += a;
            b /= 2;
        }
        return a + r;
    }
    ```