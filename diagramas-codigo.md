# Presentacion 
## Problemas resueltos en clase con DFD
### Ejercicio 1. Contar del 1 hasta el 10 y sumar los valores. (FOR)
#### 1.1 Analisis. 
Sumar los valores del 1 al 10.
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197370994-6bed5c67-531c-4b90-b360-dcf3b6189313.png)
#### 1.3 Prueba de escritorio
|s|i|i<=10|s=s+i|i++|Salida|
|-|-|-|-|-|-|
|0|1|1<=10|0+1|1+1||
|1|2|2<=10|1+2|2+1||
|3|3|3<=10|3+3|3+1||
|6|4|4<=10|6+4|4+1||
|10|5|5<=10|10+5|5+1||
|15|6|6<=10|15+6|6+1||
|21|7|7<=10|21+7|7+1||
|28|8|8<=10|28+8|8+1||
|36|9|9<=10|36+9|9+1||
|45|10|10<=10|45+10|10+1|55|
#### 1.4 Entradas.
No tiene ninguna entrada.
#### 1.5 Salidas.
55.
#### 1.6 Codigo.
```dart
void main(List<String> args) {
  int s = 0;
  for (var i = 1; i <= 10; i++) {
    s += i;
  }
  print("La suma de los valores es: $s");
}
```
### Ejercicio 2. Contar del 1 hasta el 10 y sumar los valores. (WHILE)
#### 1.1 Analisis. 
Sumar los valores del 1 al 10.
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197401601-6bc0d83e-df63-4273-ad29-1fccf8e1cf54.png)
#### 1.3 Prueba de escritorio 
|s|c|c<=10|s=s+c|c=c++|Salida|
|-|-|-|-|-|-|
|0|1|1<=10|0+1|1+1||
|1|2|2<=10|1+2|2+1||
|3|3|3<=10|3+3|3+1||
|6|4|4<=10|6+4|4+1||
|10|5|5<=10|10+5|5+1||
|15|6|6<=10|15+6|6+1||
|21|7|7<=10|21+7|7+1||
|28|8|8<=10|28+8|8+1||
|36|9|9<=10|36+9|9+1||
|45|10|10<=10|45+10|10+1|55|
#### 1.4 Entradas.
No tiene ninguna entrada.
#### 1.5 Salidas.
55.
#### 1.6 Codigo.
```dart
void main(List<String> args) {
  int s = 0, c = 1;

  while (c <= 10) {
    s += c;
    c++;
  }
  print("El resultado de la suma de los valores es:$s");
}
```
### Ejercicio 3. Contar del 1 hasta el 10 y sumar los valores. (DO-WHILE)
#### 1.1 Analisis. 
Sumar los valores del 1 al 10.
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197401840-390bcb1a-f2cb-4799-8c83-3978dd0ee754.png)
#### 1.3 Prueba de escritorio 
|s|c|s=s+c|c=c++|c<=10|Salida|
|-|-|-|-|-|-|
|0|1|0+1|1+1|2<=10||
|1|2|1+2|2+1|3<=10||
|3|3|3+3|3+1|4<=10||
|6|4|6+4|4+1|5<=10||
|10|5|10+5|5+1|6<=10||
|15|6|15+6|6+1|7<=10||
|21|7|21+7|7+1|8<=10||
|28|8|28+8|8+1|9<=10||
|36|9|36+9|9+1|10<=10||
|45|10|45+10|10+1||55|
#### 1.4 Entradas.
No tiene ninguna entrada.
#### 1.5 Salidas.
55.
#### 1.6 Codigo.
```dart
void main(List<String> args) {
  int s = 0, c = 1;

  do {
    s += c;
    c++;
  } while (c <= 10);
  print("El resultado de la suma de los valores es:$s");
}
```
### Ejercicio 4. Obtenga la suma de los primeros 5 numeros pares. (FOR)
#### 1.1 Analisis. 
Obtener los primeros 5 numeros pares y sumarlos entre si.
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197371049-0a3fe20e-11ef-4136-94b4-0d2ad7275bc2.png)
#### 1.3 Prueba de escritorio 
|s|i|i<=5|s=s+ i * 2|i++|salida|
|-|-|-|-|-|-|
|0|1|1<=5|0+ 1 * 2|1+1||
|2|2|2<=5|2+ 2 * 2|2+1||
|6|3|3<=5|6+ 3 * 2|3+1||
|12|4|4<=5|12+ 4 * 2|4+1||
|20|5|5<=5|20+ 5 * 2|5+1|30|
#### 1.4 Entradas.
No tiene ninguna entrada.
#### 1.5 Salidas.
30.
#### 1.6 Codigo.
```dart
void main(List<String> args) {
  int s = 0;
  for (var i = 2; i <= 10; i = i + 2) {
    s = s + i;
  }
  print("resultado de la suma de numeros pares es:$s");
}
```
### Ejercicio 5. Obtenga la suma de los primeros 5 numeros pares. (WHILE)
#### 1.1 Analisis.
Obtener los primeros 5 numeros pares y sumarlos entre si.
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197402064-570cad02-fbe8-4d55-bdfc-3c025b1e2286.png)
#### 1.3 Prueba de escritorio 
|s|c|c<=5|s=s+ i * 2|c++|salida|
|-|-|-|-|-|-|
|0|1|1<=5|0+ 1 * 2|1+1||
|2|2|2<=5|2+ 2 * 2|2+1||
|6|3|3<=5|6+ 3 * 2|3+1||
|12|4|4<=5|12+ 4 * 2|4+1||
|20|5|5<=5|20+ 5 * 2|5+1|30|
#### 1.4 Entradas.
No tiene ninguna entrada.
#### 1.5 Salidas.
30.
#### 1.6 Codigo.
```dart
void main(List<String> args) {
  int s = 0, c = 1;
  while (c <= 5) {
    s = s + c * 2;
    c = c + 1;
  }
  print("resultado de la suma de numeros pares:$s");
}
```
### Ejercicio 6. Obtenga la suma de los primeros 5 numeros pares. (DO-WHILE)
#### 1.1 Analisis.
Obtener los primeros 5 numeros pares y sumarlos entre si.
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197402096-75bf182b-69be-40bc-b2b7-95e5d353861c.png)
#### 1.3 Prueba de escritorio 
|s|c|s=s+ i * 2|c++|c<=5|salida|
|-|-|-|-|-|-|
|0|1|0+ 1 * 2|1+1|1<=5||
|2|2|2+ 2 * 2|2+1|2<=5||
|6|3|6+ 3 * 2|3+1|3<=5||
|12|4|12+ 4 * 2|4+1|4<=5||
|20|5|20+ 5 * 2|5+1|5<=5|30|
#### 1.4 Entradas.
No tiene ninguna entrada.
#### 1.5 Salidas.
30.
#### 1.6 Codigo.
```dart
void main(List<String> args) {
  int s = 0, c = 1;

  do {
    s = s + c * 2;
    c = c + 1;
  } while (c <= 5);
  print("la suma de numeros pares es:$s");
}
```
### Ejercicio 7. Almacene en un array el numero n leido del teclado, el tamaño del array es de 10. (FOR)
#### 1.1 Analisis. 
Debemos almacenar en 10 espacios el numero n.
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197402229-8076c2bc-525f-445e-8f57-468b827f1eeb.png)
#### 1.3 Prueba de escritorio 
|n|i|i<=9|A[i]=n|i++|
|-|-|-|-|-|
|4|0|0<=9|A[0]=4|0+1|
|4|1|1<=9|A[1]=4|1+1|
|4|2|2<=9|A[2]=4|2+1|
|4|3|3<=9|A[3]=4|3+1|
|4|4|4<=9|A[4]=4|4+1|
|4|5|5<=9|A[5]=4|5+1|
|4|6|6<=9|A[6]=4|6+1|
|4|7|7<=9|A[7]=4|7+1|
|4|8|8<=9|A[8]=4|8+1|
|4|9|9<=9|A[9]=4|9+1|
#### 1.4 Entradas.
n.
#### 1.5 Salidas.
A.
#### 1.6 Codigo.
```dart
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  for (var i = 0; i <= 9; i++) {
    String? s = stdin.readLineSync();
    if (s != null) {
      int n = int.parse(s);
      arra[i] = n;
    }
  }
  stdout.write("aqui esta la lista, $arra");
}
```
### Ejercicio 8. Almacene en un array el numero n leido del teclado, el tamaño del array es de 10. (WHILE)
#### 1.1 Analisis. 
Debemos almacenar en 10 espacios el numero n.
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197402293-bd4cc849-581f-4e8c-8638-5a9776826320.png)
#### 1.3 Prueba de escritorio 
|n|c|c<=9|A[c]=n|c++|
|-|-|-|-|-|
|7|0|0<=9|A[0]=7|0+1|
|7|1|1<=9|A[1]=7|1+1|
|7|2|2<=9|A[2]=7|2+1|
|7|3|3<=9|A[3]=7|3+1|
|7|4|4<=9|A[4]=7|4+1|
|7|5|5<=9|A[5]=7|5+1|
|7|6|6<=9|A[6]=7|6+1|
|7|7|7<=9|A[7]=7|7+1|
|7|8|8<=9|A[8]=7|8+1|
|7|9|9<=9|A[9]=7|9+1|
#### 1.4 Entradas.
n.
#### 1.5 Salidas.
A.
#### 1.6 Codigo.
```dart
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  int i = 0;
  while (i <= 9) {
    String? s = stdin.readLineSync();
    if (s != null) {
      int ner = int.parse(s);
      arra[i] = ner;
    }
    i++;
  }
  stdout.write("Tu lista es, $arra ");
}
```
### Ejercicio 9. Almacene en un array el numero n leido del teclado, el tamaño del array es de 10. (DO-WHILE)
#### 1.1 Analisis. 
Debemos almacenar en 10 espacios el numero n.
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197402325-1e3f53a4-fba0-4296-9012-44f6f9550e39.png)
#### 1.3 Prueba de escritorio 
|n|c|A[c]=n|c++|c<=9|
|-|-|-|-|-|
|5|0|0<=9|0+1|A[0]=5|
|5|1|1<=9|1+1|A[1]=5|
|5|2|2<=9|2+1|A[2]=5|
|5|3|3<=9|3+1|A[3]=5|
|5|4|4<=9|4+1|A[4]=5|
|5|5|5<=9|5+1|A[5]=5|
|5|6|6<=9|6+1|A[6]=5|
|5|7|7<=9|7+1|A[7]=5|
|5|8|8<=9|8+1|A[8]=5|
|5|9|9<=9|9+1|A[9]=5|
#### 1.4 Entradas.
n.
#### 1.5 Salidas.
A.
#### 1.6 Codigo.
```dart
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  int i = 0;
  do {
    String? s = stdin.readLineSync();
    if (s != null) {
      int n = int.parse(s);
      arra[i] = n;
      i++;
    }
  } while (i <= 9);
  stdout.write("Tu lista es $arra ");
}
```
### Ejercicio 10. Almacene los n numeros leidos del teclado en un vector de 10 elementos. (FOR)
#### 1.1 Analisis. 
Almacenar en un vector el coteo negativo del 10 a 0 en orden.
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197371156-4295ab1d-e995-4f38-8338-0bdcdac36c00.png)
#### 1.3 Prueba de escritorio 
|i|i<=9|n|A[i]=n|i+1|
|-|-|-|-|-|
|0|0<=9|6|A[0]=6|0+1|
|1|1<=9|4|A[1]=4|1+1|
|2|2<=9|8|A[2]=8|2+1|
|3|3<=9|1|A[3]=1|3+1|
|4|4<=9|4|A[4]=4|4+1|
|5|5<=9|9|A[5]=9|5+1|
|6|6<=9|2|A[6]=2|6+1|
|7|7<=9|4|A[7]=4|7+1|
|8|8<=9|3|A[8]=3|8+1|
|9|9<=9|5|A[9]=5|9+1|
#### 1.4 Entradas.
n.
#### 1.5 Salidas.
A.
#### 1.6 Codigo.
```dart
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  for (var i = 0; i <= 9; i++) {
    String? s = stdin.readLineSync();
    if (s != null) {
      int n = int.parse(s);
      arra[i] = n;
    }
  }
  stdout.write("aqui esta la lista, $arra");
}
```
### Ejercicio 11. Almacene los n numeros leidos del teclado en un vector de 10 elementos. (WHILE)
#### 1.1 Analisis. 
Almacenar en 10 espacios diferentes los numeros ingresados por el usario.
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197402477-524b88d2-dcec-414e-8015-489a0de963db.png)
#### 1.3 Prueba de escritorio 
|c|c<=9|n|A[c]=n|c+1|
|-|-|-|-|-|
|0|0<=9|4|A[0]=4|0+1|
|1|1<=9|8|A[1]=8|1+1|
|2|2<=9|9|A[2]=9|2+1|
|3|3<=9|2|A[3]=2|3+1|
|4|4<=9|4|A[4]=4|4+1|
|5|5<=9|6|A[5]=6|5+1|
|6|6<=9|1|A[6]=1|6+1|
|7|7<=9|8|A[7]=8|7+1|
|8|8<=9|7|A[8]=7|8+1|
|9|9<=9|9|A[9]=9|9+1|
#### 1.4 Entradas.
n.
#### 1.5 Salidas.
A.
#### 1.6 Codigo.
```dart
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  int i = 0;
  while (i <= 9) {
    String? s = stdin.readLineSync();
    if (s != null) {
      int ner = int.parse(s);
      arra[i] = ner;
    }
    i++;
  }
  stdout.write("Tu lista es, $arra ");
}
```
### Ejercicio 12. Almacene los n numeros leidos del teclado en un vector de 10 elementos. (DO-WHILE)
#### 1.1 Analisis. 
Almacenar en 10 espacios diferentes los numeros ingresados por el usario.
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197405036-fac206f1-3619-44c2-8c64-3fc58a899b1a.png)
#### 1.3 Prueba de escritorio 
|c|n|A[c]=n|c+1|c<=9|
|-|-|-|-|-|
|0|4|A[0]=4|0+1|0<=9|
|1|8|A[1]=8|1+1|1<=9|
|2|9|A[2]=9|2+1|2<=9|
|3|2|A[3]=2|3+1|3<=9|
|4|4|A[4]=4|4+1|4<=9|
|5|6|A[5]=6|5+1|5<=9|
|6|1|A[6]=1|6+1|6<=9|
|7|8|A[7]=8|7+1|7<=9|
|8|7|A[8]=7|8+1|8<=9|
|9|9|A[9]=9|9+1||
#### 1.4 Entradas.
#### 1.5 Salidas.
#### 1.6 Codigo.
```dart
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  int i = 0;
  do {
    String? s = stdin.readLineSync();
    if (s != null) {
      int n = int.parse(s);
      arra[i] = n;
      i++;
    }
  } while (i <= 9);
  stdout.write("Tu lista es $arra ");
}
```
### Ejercicio 13. Almacene un contador negativo en un vector, el conteo es de 10 a 0. (FOR)
#### 1.1 Analisis. 
Almacenar en 10 espacios un conteo regresivo del 10 al 0.
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197371211-333c3251-eb1f-40f0-b149-1e12870d3be7.png)
#### 1.3 Prueba de escritorio 
|i|i>=0|A[10-i]=i|i--|
|-|-|-|-|
|10|10>=0|A[10-10]=0|10-1|
|9|9>=0|A[10-9]=1|9-1|
|8|8>=0|A[10-8]=2|8-1|
|7|7>=0|A[10-7]=3|7-1|
|6|6>=0|A[10-6]=4|6-1|
|5|5>=0|A[10-5]=5|5-1|
|4|4>=0|A[10-4]=6|4-1|
|3|3>=0|A[10-3]=7|3-1|
|2|2>=0|A[10-2]=8|2-1|
|1|1>=0|A[10-1]=9|1-1|
|0|0>=0|A[10-0]=10||
#### 1.4 Entradas.
No tiene entradas.
#### 1.5 Salidas.
A.
#### 1.6 Codigo.
```dart
void main() {
  var arr = <int>[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  for (var i = 10; i >= 0; i--) {
    arr[10 - i] = i;
  }
  print(arr);
}
```
### Ejercicio 14. Almacene un contador negativo en un vector, el conteo es de 10 a 0. (WHILE)
#### 1.1 Analisis. 
Almacenar en 10 espacios un conteo regresivo del 10 al 0.
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197405073-a7e022a3-c0ef-46ed-b68a-4554b0d4759e.png)
#### 1.3 Prueba de escritorio 
|c|c>=0|A[10-c]=c|c--|
|-|-|-|-|
|10|10>=0|A[10-10]=0|10-1|
|9|9>=0|A[10-9]=1|9-1|
|8|8>=0|A[10-8]=2|8-1|
|7|7>=0|A[10-7]=3|7-1|
|6|6>=0|A[10-6]=4|6-1|
|5|5>=0|A[10-5]=5|5-1|
|4|4>=0|A[10-4]=6|4-1|
|3|3>=0|A[10-3]=7|3-1|
|2|2>=0|A[10-2]=8|2-1|
|1|1>=0|A[10-1]=9|1-1|
|0|0>=0|A[10-0]=10||
#### 1.4 Entradas.
No tiene entradas.
#### 1.5 Salidas.
A.
#### 1.6 Codigo.
```dart
void main() {
  var arr = <int>[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  int c = 10;
  while (c >= 0) {
    arr[10 - c] = c;
    c = c - 1;
  }
  print(arr);
}
```
### Ejercicio 15. Almacene un contador negativo en un vector, el conteo es de 10 a 0. (DO-WHILE)
#### 1.1 Analisis. Almacenar en 10 espacios un conteo regresivo del 10 al 0.
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197405102-c906b7b0-0bff-4638-8fce-a677a3c4b865.png)
#### 1.3 Prueba de escritorio 
|c|A[10-c]=c|c--|c>=0|
|-|-|-|-|
|10|A[10-10]=0|10-1|10>=0|
|9|A[10-9]=1|9-1|9>=0|
|8|A[10-8]=2|8-1|8>=0|
|7|A[10-7]=3|7-1|7>=0|
|6|A[10-6]=4|6-1|6>=0|
|5|A[10-5]=5|5-1|5>=0|
|4|A[10-4]=6|4-1|4>=0|
|3|A[10-3]=7|3-1|3>=0|
|2|A[10-2]=8|2-1|2>=0|
|1|A[10-1]=9|1-1|1>=0|
|0|A[10-0]=10||0>=0|
#### 1.4 Entradas.
No tiene entradas.
#### 1.5 Salidas.
A.
#### 1.6 Codigo.
```dart
void main() {
  var arr = <int>[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  int c = 10;
  do {
    arr[10 - c] = c;
    c = c - 1;
  } while (c >= 0);
  print(arr);
}
```
### Ejercicio 16. Almacene en un vector de tamaño 10, todos los numeros pares capturados hasta completar todos. (FOR)
#### 1.1 Analisis. 
Tenemos que insertar numero pares y almacenarlos en 10 espacios.
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197382216-7f05339c-b12f-4d84-9978-8caa04a7534f.png)
#### 1.3 Prueba de escritorio 
|i|i<=9|n|n%2==0|A[i]=n|i+1|
|-|-|-|-|-|-|
|0|0<=9|8|8%2==0|A[0]=8|0+1|
|1|1<=9|4|4%2==0|A[1]=4|1+1|
|2|2<=9|2|2%2==0|A[2]=2|2+1|
|3|3<=9|8|8%2==0|A[3]=8|3+1|
|4|4<=9|2|4%2==0|A[4]=2|4+1|
|5|5<=9|6|6%2==0|A[5]=6|5+1|
|6|6<=9|6|6%2==0|A[6]=6|6+1|
|7|7<=9|2|2%2==0|A[7]=2|7+1|
|8|8<=9|4|4%2==0|A[8]=4|8+1|
|9|9<=9|4|4%2==0|A[9]=4|9+1|
#### 1.4 Entradas.
n.
#### 1.5 Salidas.
A.
#### 1.6 Codigo.
```py
numeros = [2, 4, 6, 8, 10, 12, 14, 16, 18, 20]

def extraer_pares(lista):
    pares = []

    for n in lista:
        if n % 2 == 0:
            pares.append(n)

    return pares

print()

resultado = extraer_pares(numeros)

print("Contenido de la variable`resultado`:", resultado)
print("Cantidad de elementos en la lista `resultado`:", len(resultado))
```
### Ejercicio 17. Almacene en un vector de tamaño 10, todos los numeros pares capturados hasta completar todos. (WHILE)
#### 1.1 Analisis. 
Tenemos que insertar numero pares y almacenarlos en 10 espacios.
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197382230-a9f1f438-30d8-44c4-9d04-78c41acc7111.png)
#### 1.3 Prueba de escritorio 
|c|c<=9|n|n%2==0|A[c]=n|c+1|
|-|-|-|-|-|-|
|0|0<=9|2|8%2==0|A[0]=2|0+1|
|1|1<=9|4|4%2==0|A[1]=4|1+1|
|2|2<=9|6|2%2==0|A[2]=6|2+1|
|3|3<=9|8|8%2==0|A[3]=8|3+1|
|4|4<=9|2|4%2==0|A[4]=2|4+1|
|5|5<=9|4|6%2==0|A[5]=4|5+1|
|6|6<=9|6|6%2==0|A[6]=6|6+1|
|7|7<=9|8|2%2==0|A[7]=8|7+1|
|8|8<=9|2|4%2==0|A[8]=2|8+1|
|9|9<=9|4|4%2==0|A[9]=4|9+1|
#### 1.4 Entradas.
n.
#### 1.5 Salidas.
A.
#### 1.6 Codigo.
```py
numeros = [2, 4, 6, 8, 10, 12, 14, 16, 18, 20]
def extraer_pares(lista):
    pares = []

    for n in lista:
        if n % 2 == 0:
            pares.append(n)

    return pares

print()

resultado = extraer_pares(numeros)

print("Contenido de la variable`resultado`:", resultado)
print("Cantidad de elementos en la lista `resultado`:", len(resultado))
```
### Ejercicio 18. Almacene en un vector de tamaño 10, todos los numeros pares capturados hasta completar todos. (DO-WHILE)
#### 1.1 Analisis. 
Tenemos que insertar numero pares y almacenarlos en 10 espacios.
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197382249-ea63e694-11ef-47fc-bf5b-5f4173ad7766.png)
#### 1.3 Prueba de escritorio 
|c|n|n%2==0|A[c]=n|c+1|c<=9|
|-|-|-|-|-|-|
|0|2|8%2==0|A[0]=2|0+1|0<=9|
|1|2|4%2==0|A[1]=2|1+1|1<=9|
|2|4|2%2==0|A[2]=4|2+1|2<=9|
|3|4|8%2==0|A[3]=4|3+1|3<=9|
|4|6|4%2==0|A[4]=6|4+1|4<=9|
|5|6|6%2==0|A[5]=6|5+1|5<=9|
|6|8|6%2==0|A[6]=8|6+1|6<=9|
|7|8|2%2==0|A[7]=8|7+1|7<=9|
|8|2|4%2==0|A[8]=2|8+1|8<=9|
|9|2|4%2==0|A[9]=2|9+1|9<=9|
#### 1.4 Entradas.
n.
#### 1.5 Salidas.
A.
#### 1.6 Codigo.
```dart
import 'dart:io';
import 'dart:async';

void main() {
  var array = [];
  var c = 0;
  do {
    int n = int.parse(stdin.readLineSync()!);

    if (n % 2 == 0) {
      array.add(n);
      c = c + 1;
    }
  } while (c <= 9);
  print(array);
}
```
### Ejercicio 19. Obtener el promedio de las calificaciones aprobatorias y la cantidad de alumnos reprobados. La calificación entre 0 y 10 y el maximo de alumnos es de 15. (FOR)
#### 1.1 Analisis.
Sumar las calificaiones de los alumnos aprobados y sacarles el promedio, despues contar la cantidad de reprobados mayores a 5.
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197411505-2a259b71-368e-4ae0-8399-d6c445b9b111.png)
#### 1.3 Prueba de escritorio 
|i|i<=14|Cal|Cal>=LI|Cal<=LS|A[i]=Cal|i+1|Cal<5|S_A=S_A+Cal|C_A=C_A+1|C_R++|P_A=S_A/C_A|P_A|C_R|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
|0|0<=14|7|7>=0|7<=10|A[0]=7|0+1|7<5|0+7|0+1|||||
|1|1<=14|6|6>=0|6<=10|A[1]=6|1+1|6<5|7+6|1+1|||||
|2|2<=14|3|3>=0|3<=10|A[2]=3|2+1||||0+1||||
|3|3<=14|9|9>=0|9<=10|A[3]=9|3+1|9<5|13+9|2+1|||||
|4|4<=14|9|9>=0|9<=10|A[4]=9|4+1|9<5|22+9|3+1|||||
|5|5<=14|10|10>=0|10<=10|A[5]=10|5+1|10<5|31+10|4+1|||||
|6|6<=14|5|5>=0|5<=10|A[6]=5|6+1||||1+1||||
|7|7<=14|10|10>=0|10<=10|A[7]=10|7+1|10<5|41+10|5+1|||||
|8|8<=14|8|8>=0|8<=10|A[8]=8|8+1|8<5|51+8|6+1|||||
|9|9<=14|7|7>=0|7<=10|A[9]=7|9+1|7<5|59+7|7+1|||||
|10|10<=14|9|9>=0|9<=10|A[10]=9|10+1|9<5|66+9|8+1|||||
|11|11<=14|4|4>=0|4<=10|A[11]=4|11+1||||2+1||||
|12|12<=14|10|10>=0|10<=10|A[12]=10|12+1|10<5|75+10|9+1|||||
|13|13<=14|9|9>=0|9<=10|A[13]=9|13+1|9<5|85+9|10+1|||||
|14|14<=14|8|8>=0|8<=10|A[14]=8|14+1|8<5|94+8|11+1||P_A=102/12|8.5|3|
#### 1.4 Entradas.
Cal.
#### 1.5 Salidas.
P_A; C_R.
#### 1.6 Codigo.
```py
alumnos = list(range(15))
p_aprobados = 0
j = 0

for i in alumnos: 
    while(True):
        calificacion = int(input("Ingresa la calificación >>"))
        if (calificacion >= 0 and calificacion <= 10):
            break
        else:
            print("Calificación fuera de rango. Intenta de nuevo")
 
    if (calificacion < 6):
     alumnos[i] = "R"
    else:
     p_aprobados = calificacion + p_aprobados
     j = j + 1
     alumnos[i] = "A"

print("\033[33;1m",alumnos,"\033[39m")
print("El promedio de calificación de los aprobados es de >>",round(p_aprobados/j,2))
print("El total de aprobados fueron >> ",j)
print("El total de reprobados fueron >> ",(len(alumnos)-j))
```
### Ejercicio 20. Obtener el promedio de las calificaciones aprobatorias y la cantidad de alumnos reprobados. La calificación entre 0 y 10 y el maximo de alumnos es de 15. (WHILE)
#### 1.1 Analisis. 
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197417109-b6f776ed-9408-4a55-ab89-fb0fe7bf07c2.png)
#### 1.3 Prueba de escritorio 
|C_Almn|C_Almn<=14|Cal|Cal>=LI|Cal<=LS|A[i]=Cal|i+1|Cal<5|S_A=S_A+Cal|C_A=C_A+1|C_R++|P_A=S_A/C_A|P_A|C_R|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
|0|0<=14|6|6>=0|6<=10|A[0]=6|0+1|6<5|0+6|0+1|||||
|1|1<=14|6|6>=0|6<=10|A[1]=6|1+1|6<5|7+6|1+1|||||
|2|2<=14|2|2>=0|2<=10|A[2]=2|2+1||||0+1||||
|3|3<=14|4|4>=0|4<=10|A[3]=4|3+1||||1+1||||
|4|4<=14|9|9>=0|9<=10|A[4]=9|4+1|9<5|22+9|3+1|||||
|5|5<=14|10|10>=0|10<=10|A[5]=10|5+1|10<5|31+10|4+1|||||
|6|6<=14|5|5>=0|5<=10|A[6]=5|6+1||||1+1||||
|7|7<=14|3|3>=0|3<=10|A[7]=3|7+1||||2+1||||
|8|8<=14|8|8>=0|8<=10|A[8]=8|8+1|8<5|51+8|6+1|||||
|9|9<=14|7|7>=0|7<=10|A[9]=7|9+1|7<5|59+7|7+1|||||
|10|10<=14|9|9>=0|9<=10|A[10]=9|10+1|9<5|66+9|8+1|||||
|11|11<=14|4|4>=0|4<=10|A[11]=4|11+1||||2+1||||
|12|12<=14|10|10>=0|10<=10|A[12]=10|12+1|10<5|75+10|9+1|||||
|13|13<=14|9|9>=0|9<=10|A[13]=9|13+1|9<5|85+9|10+1|||||
|14|14<=14|8|8>=0|8<=10|A[14]=8|14+1|8<5|94+8|11+1||P_A=102/12|8.5|3|
#### 1.4 Entradas.
Cal.
#### 1.5 Salidas.
P_A; C_R.
#### 1.6 Codigo.
```py
alumnos = list(range(15))
p_aprobados = 0
j = 0

for i in alumnos: 
    while(True):
        calificacion = int(input("Ingresa la calificación >>"))
        if (calificacion >= 0 and calificacion <= 10):
            break
        else:
            print("Calificación fuera de rango. Intenta de nuevo")
 
    if (calificacion < 6):
     alumnos[i] = "R"
    else:
     p_aprobados = calificacion + p_aprobados
     j = j + 1
     alumnos[i] = "A"

print("\033[33;1m",alumnos,"\033[39m")
print("El promedio de calificación de los aprobados es de >>",round(p_aprobados/j,2))
print("El total de aprobados fueron >> ",j)
print("El total de reprobados fueron >> ",(len(alumnos)-j))
```
### Ejercicio 21. Obtener el promedio de las calificaciones aprobatorias y la cantidad de alumnos reprobados. La calificación entre 0 y 10 y el maximo de alumnos es de 15. (DO-WHILE)
#### 1.1 Analisis. 
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197417134-8b3fa286-832c-4ac4-a678-80d6132d225d.png)
#### 1.3 Prueba de escritorio 
|C_Almn|Cal|Cal>=LI|Cal<=LS|A[i]=Cal|i++|Cal<5|S_A=S_A+Cal|C_A=C_A+1|C_R++|C_Almn<=14|P_A=S_A/C_A|P_A|C_R|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
|0|6|6>=0|6<=10|A[0]=6|0+1|6<5|0+6|0+1||1<=14||||
|1|4|4>=0|4<=10|A[1]=4|1+1||||0+1|2<=14||||
|2|9|9>=0|9<=10|A[2]=9|2+1|9<5|6+9|1+1||3<=14||||
|3|5|5>=0|5<=10|A[3]=5|3+1||||1+1|4<=14||||
|4|8|8>=0|8<=10|A[4]=8|4+1|8<5|15+8|2+1||5<=14||||
|5|4|4>=0|4<=10|A[5]=4|5+1||||2+1|6<=14||||
|6|7|7>=0|7<=10|A[6]=7|6+1|7<5|23+7|3+1||7<=14||||
|7|2|2>=0|2<=10|A[7]=2|7+1||||3+1|8<=14||||
|8|9|9>=0|9<=10|A[8]=9|8+1|9<5|30+9|4+1||9<=14||||
|9|1|1>=0|1<=10|A[9]=1|9+1||||4+1|10<=14||||
|10|10|10>=0|10<=10|A[10]=10|10+1|10<5|39+10|5+1||11<=14||||
|11|4|4>=0|4<=10|A[11]=4|11+1||||5+1|12<=14||||
|12|9|9>=0|9<=10|A[12]=9|12+1|9<5|49+9|6+1||13<=14||||
|13|5|5>=0|5<=10|A[13]=5|13+1||||6+1|14<=14||||
|14|9|9>=0|9<=10|A[14]=9|14+1|9<5|58+9|7+1|||P_A=67/8|8.3|7|
#### 1.4 Entradas.
Cal.
#### 1.5 Salidas.
P_A; C_R.
#### 1.6 Codigo.
```dart
import 'dart:io';
import 'dart:async';

void main() {
  double PromA = 0;
  var contr = 0;
  double sumaA = 0;
  double contA = 0;
  double cal1 = 0;
  double cal2 = 1;
  var cont = 0;
  stdout.write("Dame las calificaciones\n ");
  stdout.write("----------\n");
  do {
    double c = double.parse(stdin.readLineSync()!);
    cont = cont +1;
    if (c > 10) {
      print('La calificacion no puede ser mayor a 10');
      cont = cont - 1;
    }
    if (c < 0) {
      print('La calificacion no puede ser menor a 0');
      cont = cont - 1;
    }
    if (c < 6 && c > 0) {
      contr = contr + 1;
    }
    if (c <= 10 && c >= 6) {
      cal1 = c;
      sumaA = sumaA + cal1;
      contA++;
    }
    if (cal1 > cal2) {
      cal2 = cal1;
    }
  } while (cont <= 14);
  PromA = sumaA / contA;
  print('El promedio de aprobados es $PromA');
  print('La calificacion mas alta es $cal2');
  print('La cantidad de reprobados son $contr');
}
```
### Ejercicio 22. 
#### 1.1 Analisis. 
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197482355-9109f57f-e07a-47fa-9097-ef04e9e0a386.png)
#### 1.3 Prueba de escritorio 
#### 1.4 Entradas.
#### 1.5 Salidas.
#### 1.6 Codigo.
```py
sp=0
cp=0
pp=0
si=0
ci=0
pi=0
li=-1
ls=-1
n=-1
num=-1

while(li<0):
    li = int(input("Limite inferior: "))
    
    if(li<0):
        print("Tiene que ser mayor a 0")
        
while(ls<li):
    ls = int(input("Limite superior: "))
    
    if(ls<li):
        print("Tiene que ser mayor que el limite inferior")
        
while(n<0):
    n = int(input("¿Cuantos numeros? "))
    
    if(n<0):
        print("Tiene que ser mayor a 0")
    
for i in range(n): 
    while(num<=li or num>=ls):
        num = int(input("Dame un numero de LI y LS: "))
        
        if(num<=li or num>=ls):
            print("Tiene que estar dentro del LI al LS")

    if(num%2==0):
        sp=sp+num
        cp=cp+1
    else:
        si=si+num
        ci=ci+1
        
    num=-1       
         
if(sp==0 or cp==0):
    pp=0
else:
    pp=sp/cp
    
if(si==0 or ci==0):
    pi=0
else:
    pi=si/ci
    
if(pp>pi):
    print("El PP es mayor que el PI")
else:
    print("El PI es mayor que el PP")
```
### Ejercicio 23. 
#### 1.1 Analisis. 
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197482559-3f9d511c-a368-4b92-8f2b-b4ff3bd22178.png)
#### 1.3 Prueba de escritorio 
#### 1.4 Entradas.
#### 1.5 Salidas.
#### 1.6 Codigo.
```py
print("Dame Límite inferior: ")
Li = int(input())
while Li<0:
    print("El límite inferior debe ser mayor a 0")
    print("Dame Límite inferior: ")
    Li = int(input())

print("Dame límite superior: ")
Ls = int(input())
while Ls<=Li:
    print("El límite superior no puede ser menor o igual al limite inferior")
    print("Dame límite superior: ")
    Ls = int(input())

pares = 0
impares = 0

lista=[]
for x in range(10):
    valor=int(input("Ingrese un valor entero: "))
    lista.append(valor)
print(lista)

for a in lista:
    if a % 2 == 0:
        pares = pares + a
    else:
        impares = impares + a
print("La suma de los números pares es: ",pares)
print("La suma de los números impares es: ",impares)

prom_pares = pares / a
prom_impares = impares / a

print("El promedio de los números pares es: ",prom_pares)
print("El promedio de los números impares es: ",prom_impares)

if prom_pares > prom_impares:
    print("El promedio de los pares es mayor que el promedio de los impares.")
else:
    print("El promedio de los números impares es mayor que el promedio de los pares.")
```
### Ejercicio 24. 
#### 1.1 Analisis. 
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197482488-8151b935-fc88-4412-bd5f-091a6f20aa66.png)
#### 1.3 Prueba de escritorio 
#### 1.4 Entradas.
#### 1.5 Salidas.
#### 1.6 Codigo.
```dar
import 'dart:io';

void main() {
  double sumap = 0;
  double sumai = 0;
  var contp = 0;
  var conti = 0;
  double promp = 0;
  double promi = 0;
  print('Introduce el limite inferior, mayor a 0');
  var li = int.parse(stdin.readLineSync()!);
  if (li < 0) {
    print('tu limite inferior debe ser mayor a 0');
  }
  if (li > 0) {
    print('Ahora introduce un limite superior');
    var ls = int.parse(stdin.readLineSync()!);
    if (ls < li) {
      print('tu limite superior debe ser mayor a tu limite inferior');
    }
    var cont = li;
    do {
      if (cont <= ls) {
        sumai = sumai + cont;
        conti = conti + 1;
      }
      if (cont % 2 == 0) {
        sumap = sumap + cont;
        contp = contp + 1;
        sumai = sumai - cont;
        conti = conti - 1;
      }
      cont = cont + 1;
    } while (cont <= ls);

    promi = sumai / conti;
    print('los impares son $conti y su promedio es $promi');
    promp = sumap / contp;
    print('los pares son $contp y su promedio es $promp');
    if (promp < promi) {
      print('$promi es mayor');
    }
    if (promp > promi) {
      print('el promedio $promp es mayor');
    }
  }
}
```
### Ejercicio 25. 
#### 1.1 Analisis. 
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197482672-6eed242b-d874-4e2c-8799-0594adfa0c0f.png)
#### 1.3 Prueba de escritorio 
#### 1.4 Entradas.
#### 1.5 Salidas.
#### 1.6 Codigo.
```py
Calificaciones=int(input("Ingrese la cantidad de calificaciones"))
vec=[]
n=0

for i in range(1,Calificaciones+1):
    calificacion=int(input("Calificacion: "))
    n=n+calificacion
    vec.append(calificacion)

promedio=n/len(vec)

npromedio=0
for j in vec:
    if j>promedio:
        npromedio=npromedio+1

aprobado=0

#Primero inicializas el contador
promedioAprobados = 0
for h in vec:
    if h>5:
        aprobado=aprobado+1
        #Va sumando cada unas de las notas
        promedioAprobados = promedioAprobados + h

#Luego saca el promedio sumatoria / cantidad de aprobados 
promedioAprobados = promedioAprobados / aprobado

reprobado=0
for k in vec:
    if k<5:
        reprobado=reprobado+1

print("Max Calificacion", max(vec))
print("Min calificacion", min(vec))
print("Promedio:", promedio)
print("Superiores a promedio:", npromedio)
print("Cantidad de aprobados:", aprobado)
print("Promedio de aprobados:", promedioAprobados)
print("Desaprobados:", reprobado)
```
### Ejercicio 26. 
#### 1.1 Analisis. 
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197482760-4bd30e29-9b13-4fe5-9390-3aa8e01f6411.png)
#### 1.3 Prueba de escritorio 
#### 1.4 Entradas.
#### 1.5 Salidas.
#### 1.6 Codigo.
```py
Calificaciones=int(input("Ingrese la cantidad de calificaciones"))
vec=[]
n=0
cont = 0
while(cont < Calificaciones):
    calificacion=int(input("Calificacion: "))
    n=n+calificacion
    vec.append(calificacion)
    cont += 1

promedio=n/len(vec)

npromedio=0
for j in vec:
    if j>promedio:
        npromedio=npromedio+1

aprobado=0

#Primero inicializas el contador
promedioAprobados = 0
for h in vec:
    if h>5:
        aprobado=aprobado+1
        #Va sumando cada unas de las notas
        promedioAprobados = promedioAprobados + h

#Luego saca el promedio sumatoria / cantidad de aprobados 
promedioAprobados = promedioAprobados / aprobado

reprobado=0
for k in vec:
    if k<5:
        reprobado=reprobado+1

print("Max Calificacion", max(vec))
print("Min calificacion", min(vec))
print("Promedio:", promedio)
print("Superiores a promedio:", npromedio)
print("Cantidad de aprobados:", aprobado)
print("Promedio de aprobados:", promedioAprobados)
print("Desaprobados:", reprobado)
```
### Ejercicio 27. 
#### 1.1 Analisis. 
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197482934-840febba-0be4-4fe0-9c27-281d562999aa.png)
#### 1.3 Prueba de escritorio 
#### 1.4 Entradas.
#### 1.5 Salidas.
#### 1.6 Codigo.
```py
Calificaciones=int(input("Ingrese la cantidad de calificaciones"))
vec=[]
n=0

cont = 0
while(True):
    calificacion=int(input("Calificacion: "))
    n=n+calificacion
    vec.append(calificacion)
    cont += 1
    if(cont>=Calificaciones):
        break;
        
aprobado=0

promedioAprobados = 0
for h in vec:
    if h>=5:
        aprobado=aprobado+1
        promedioAprobados = promedioAprobados + h

promedioAprobados = promedioAprobados / aprobado

reprobado=0
for k in vec:
    if k<=5:
        reprobado=reprobado+1

print("Cantidad de aprobados:", aprobado)
print("Cantidad de reprobados:", reprobado)
print("Promedio de aprobados:", promedioAprobados)
```

### Ejercicio 28. 
#### 1.1 Analisis. 
#### 1.2 DFD.
![image](https://user-images.githubusercontent.com/113395327/197483146-55c5bd23-3545-4372-b004-843558fc1981.png)
#### 1.3 Prueba de escritorio 
#### 1.4 Entradas.
#### 1.5 Salidas.
#### 1.6 Codigo.
```py
lista = [10]
cant = int(input("¿Cuantos numeros desea capturar?"))
i=1
while i <= cant:
    n = int(input(f"{i} Ingrese un numero: "))
    lista.append(n)
    i+=1

print("Numero mayor es ",max(lista))
print("Numero menor es ",min(lista))
```

### Ejercicio 29. 
#### 1.1 Analisis. 
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197483758-f4ea6e26-8ab1-4dd7-8bc4-37658cb6fc93.png)
#### 1.3 Prueba de escritorio 
#### 1.4 Entradas.
#### 1.5 Salidas.
#### 1.6 Codigo.
```dart
import 'dart:io';
import 'dart:core';

void main() {
  var Re = 0;
  var mayor = 0;
  stdout.write('Ingresa tus numeros \n');
  var lista = List.filled(10, 0);
  for (var i = 0; i <= 9; i++) {
    int Entrada = int.parse(stdin.readLineSync()!);
    lista[i] = Entrada;
  }
  var diferencias = List.filled(9, 0);
  for (var j = 0; j <= 8; j++) {
    diferencias[j] = (lista[j] - lista[j + 1]);
  }
  mayor = diferencias[0];
  for (var k = 0; k <= 8; k++) {
    if (mayor < diferencias[k]) {
      mayor = diferencias[k];
    } else {}
  }
  stdout.write("Tu lista es ");
  print(lista);
  stdout.write("y sus diferencias son ");
  print(diferencias);
  print('La diferencia mayor es ');
  print(mayor);
}
```

### Ejercicio 30. 
#### 1.1 Analisis. 
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197483811-31f1c1c8-3223-41b1-a71a-02bd0ecb54dc.png)
#### 1.3 Prueba de escritorio 
#### 1.4 Entradas.
#### 1.5 Salidas.
#### 1.6 Codigo.
```dart
import 'dart:io';

void main(List<String> args) {
  var array = [];
  int n = int.parse(stdin.readLineSync()!);
  for (var i = 0; i < 11; i++) {
    array.add(i);
    array[i] = n * i;
  }
  print('$array');
}
```

### Ejercicio 31. 
#### 1.1 Analisis. 
#### 1.2 DFD
![image](https://user-images.githubusercontent.com/113395327/197483869-000b9f97-54a5-4fa8-b514-fc84528984c0.png)
#### 1.3 Prueba de escritorio 
|i|i<=5|i++|j|j<i|j++|salida|
|-|-|-|-|-|-|-|
|1|1<=5|1+1|1|1<1|j++||
|2|2<=5|2+1|2|2<1|j++||
|3|3<=5|3+1|3|3<1|j++||
|4|4<=5|4+1|4|4<1|j++||
|5|5<=5|5+1|5|5<1|j++|salida|
#### 1.4 Entradas.
#### 1.5 Salidas.
#### 1.6 Codigo.
```dart
import 'dart:io';

void main() {
  var n = 5;
  for (var i = 1; i <= 5; i++) {
    for (var j = 1; j <= i; j++) {
      stdout.write('*');
    }
    print('');
  }
}
```
