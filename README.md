# 🧬🧪 AminoLab Software: Traductor de DNA a Proteína

Bienvenido/a a este repositorio. AminoLab es un programa escrito en Python que permite traducir secuencias de ADN a proteínas utilizando el código genético *estándar*.
Convierte las bases nitrogenadas de ADN (`A`, `T`, `C`, `G`) a ARN mensajero (`A`, `U`, `C`, `G`), busca el codón de inicio y lo traduce en aminoácidos hasta el primer codón de parada.

## 🤓 ¿Cómo usar este repositorio?
1. Clona este repositorio a través de tu terminal:

		git clone https://github.com/Yannisavlonitis/AminoLab.git


2. Desde la carpeta donde está contenido el programa, ejecútalo de la siguiente manera:

   		python AminoLab.py

3. El programa te pedirá tu secuencia de DNA, escríbela o pégala a continuación.

   		Inserta una secuencia de DNA: tu_secuencia_de_DNA


### ⚙️ Funcionamiento

1. **Entrada (`dna`)**  
   Lista con una o más secuencias de ADN.

   > ⚠️ **👀 - OJO: Secuencias de menos de 700b!!!** ⚠️  A partir de ahí, el código puede empezar a fallar :(
   
   Ejemplo:
   ```python
   dna = ['ATGGCTGACGTTGAGGCTTACCTGGAGGAGCTGGTGCTGCTGGAGCTGACCTGGGACTTAA']
3.  Código genético (inv)
  Diccionario que asocia cada aminoácido con sus codones.
  Incluye:

          'Z': codones de inicio (AUG, CUG, UUG)
  
          'X': codones de parada (UAA, UAG, UGA)

4. Salida. 
  Lista con las proteínas traducidas o un mensaje de error si la secuencia no puede traducirse (no ha encontrado un codón de iniciación).

### 🧠 Lógica del programa:

-> Convierte las bases de ADN (T) en bases de ARN (U).

-> Elimina caracteres no válidos o espacios.

-> Asegura que la secuencia sea múltiplo de 3 eliminando los sobrantes.

-> Busca el primer codón de inicio (AUG, CUG, UUG).

-> Traduce de tres en tres bases hasta encontrar un codón de parada (UAA, UAG, UGA).

-> Devuelve la secuencia de aminoácidos obtenida.

## 📚 Contenidos del repositorio

**1️⃣ - AminoLab Software**

Es el programa, desarrollado en python, que convierte una secuencia de DNA en la secuencia correspondiente de aminoácidos.

> Autor: Virginia García-Loygorri Arias

**2️⃣ - Secuencias de DNA de ejemplo**

Esta carpeta contiene secuencias de ADN que pueden usarse para probar el funcionamiento del programa AminoLab.
Incluye ejemplos sencillos, fragmentos de genes humanos y simulaciones de mutaciones puntuales.

> Autor: Tamara Noya Mosquera

**3️⃣ - Documentación**

Archivos y documentación de apoyo por si hay que refrescar los conceptos de biología o de programación.

#### 🐍 Python

Introducción a la lógica de programación y al lenguaje Python.

> Autor: Samuel Pintos González

#### 🧬 Genética clínica y de poblaciones

Conceptos de genética para que no te pierdas.

> Autor: Yannis Avlonitis Egea

#### 💻 Fundamentos de linux

Comandos y uso de la terminal para que puedas automatizar trabajos.

> Autor: Rita Pellissa Valera

#### 🪄 Secuenciación y ómicas de próxima generación

Técnicas útiles en bioinformática.

> Autor: Teresa Carrión Mera

#### 🗂 Bases de datos de genes, mRNAs y proteínas

Para que tengas dónde buscar secuencias.

> Autor: Vanesa de las Heras Hermosilla


## ⚙️ Requisitos

-> Conocimientos básicos de biología molecular.

-> Ordenador con conexión a internet.

-> Entorno Python.


## 🤝 Contribuciones

Las aportaciones son **bienvenidas** ✨
Si encuentras errores o quieres mejorar el contenido, abre un *issue* o envía un *pull request*.

## 📄 Licencia

Este proyecto está bajo la licencia [GNU Public License v3.0](https://www.gnu.org/licenses/gpl-3.0.html).

> Hemos decicido aplicar una licencia GNU para asegurar que nuestro software AminoLab sea accesible y gratis para todos los usuarios.
> Creemos firmemente en el open-access para el avance de la comunidad científica.
