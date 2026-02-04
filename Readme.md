# Implementación de Cifrados ASCII y Base64 en Python

## Descripción

Este proyecto implementa distintos mecanismos de cifrado y codificación utilizando únicamente Python básico y el conjunto de caracteres ASCII. El objetivo principal es comprender cómo funcionan los cifrados clásicos y modernos a bajo nivel, sin el uso de librerías criptográficas externas.

El archivo principal (`main.py` / `main.ipynb`) integra cifrados, generación de llaves y codificación Base64, todos desarrollados con fines académicos.

---

## Objetivos del Proyecto

El proyecto cumple con los siguientes objetivos:

- Implementar cifrados clásicos usando ASCII
- Generar llaves dinámicas a partir de texto
- Crear cifrados con llaves de tamaño fijo
- Crear cifrados con llaves de tamaño dinámico
- Implementar el algoritmo Base64 sin usar librerías externas
- Analizar la representación binaria de los datos

---

## Funcionalidades Implementadas

### 1. Generación de Llaves Dinámicas (ASCII)

Se implementa un mecanismo para generar llaves dinámicas basadas en caracteres ASCII.

**Características**
- Las llaves se generan a partir de texto o parámetros de entrada
- Cada carácter de la llave corresponde a un valor ASCII
- Permite reutilización y expansión de la llave

Este enfoque es fundamental para cifrados polialfabéticos.

---

### 2. Cifrado ASCII con Llave de Tamaño Fijo

Se implementa un cifrado en el cual:
- La llave `k` tiene un tamaño fijo
- Cada carácter del texto se cifra usando el valor ASCII correspondiente de la llave
- Se utiliza aritmética modular para mantener los valores dentro del rango ASCII

Este método permite observar el comportamiento de un cifrado por sustitución controlada.

---

### 3. Cifrado ASCII con Llave de Tamaño Dinámico

Se implementa un cifrado más robusto donde:
- La llave se ajusta dinámicamente al tamaño del mensaje
- La llave se repite o se genera en función del texto
- Cada carácter se cifra con un desplazamiento distinto

Este enfoque es similar a un cifrado de Vigenère aplicado sobre ASCII.

---

### 4. Cifrado César en ASCII

El cifrado César se implementa utilizando valores ASCII y desplazamiento modular.

**Características**
- Opera sobre letras minúsculas
- Conserva caracteres no alfabéticos
- Utiliza desplazamiento fijo

---

### 5. Implementación Manual de Base64

Se implementa el algoritmo Base64 sin utilizar la librería estándar.

**Incluye**
- Conversión ASCII a binario
- Agrupación en bloques de 6 bits
- Tabla Base64 explícita
- Padding `=`
- Decodificación a bytes

---

### 6. Representación Binaria

El proyecto incluye funciones para:
- Convertir valores decimales a binario
- Mostrar la representación binaria de caracteres ASCII
- Analizar la codificación Base64 a nivel de bits

---

## Flujo General del Programa

1. Se define un texto ASCII de entrada
2. Se genera una llave fija o dinámica
3. Se cifra el texto utilizando ASCII
4. El resultado se puede codificar en Base64
5. Se analiza la representación binaria del resultado
6. Se muestran los valores obtenidos por pantalla

---

## Requisitos

- Python 3.x

---

