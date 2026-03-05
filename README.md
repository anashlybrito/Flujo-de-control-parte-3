#Flujo de control parte 3
// Flujo de control parte 3.cpp : Este archivo contiene la función "main". La ejecución del programa comienza y termina ahí.
//

#include <iostream>
using namespace std;

int main()
{
    int n;
    int numero;
    int positivos = 0;
    int negativos = 0;
    int pares = 0;
    int impares = 0;
    
    cout << "Cantidad de numeros a ingresar: ";
    cin >> n;

    for (int i = 1; i <= n; i++) {
        cout << "Ingresar numero: " << i << ": ";
        cin >> numero;

        // positivos y negativos
        if (numero > 0) {
            positivos++;
        }
        else if (numero < 0) {
            negativos++;
        }

        // pares y impares
        if (numero % 2 == 0) {
            pares++;
        }
        else {
            impares++;
        }
    }

    cout << "Resultados:/n";
    cout << "numeros positivos: " << positivos << endl;
    cout << "numeros negativos: " << negativos << endl;
    cout << "numeros pares: " << pares << endl;
    cout << "numeros impares: " << impares << endl;

        return 0;
}

    return 0;
}
