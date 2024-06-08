# Punteros-Lenguaje-C - Ejemplo
#include <stdio.h>

// Función que intercambia los valores de dos variables usando paso por referencia
void swap(int *a, int *b) {
    int temp = *a;
    *a = *b;
    *b = temp;
}

int main() {
    int x = 10, y = 20;

    printf("Antes del intercambio: x = %d, y = %d\n", x, y);

    // Llamada a la función swap pasando las direcciones de x y y
    swap(&x, &y);

    printf("Después del intercambio: x = %d, y = %d\n", x, y);

    return 0;
}
