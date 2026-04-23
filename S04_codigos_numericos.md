# 📘 Clase: Códigos en Circuitos Digitales

---

## 1. 🔢 Códigos Numéricos

Los **códigos numéricos** permiten representar información decimal en sistemas digitales.

### 1.1 Binarios Ponderados
Cada bit tiene un **peso fijo**.

#### Ejemplos:
- **8421 (BCD natural)**
- **2421**
- **5211**

#### Características:
- Fácil conversión a decimal
- Uso común en sistemas digitales

#### Ejemplo (8421):
Decimal 9 → 1001  
(8 + 0 + 0 + 1 = 9)

---

### 1.2 Binarios No Ponderados
No existe un peso fijo por bit.

#### Ejemplos:
- Código Gray
- Exceso-3

#### Características:
- Reducen errores en transiciones
- Útiles en sistemas de medición y posicionamiento

---

## 2. ⚙️ Características y Criterios de Selección

Al elegir un código numérico, se consideran:

### ✔️ Criterios:
- Facilidad de implementación
- Número de bits requeridos
- Capacidad de detección de errores
- Velocidad de procesamiento
- Compatibilidad con sistemas existentes

### ✔️ Características importantes:
- Redundancia
- Auto-complementariedad
- Distancia de Hamming
- Simplicidad lógica

---

## 3. 🔤 Códigos Importantes

### 3.1 BCD (Binary Coded Decimal)

Representa cada dígito decimal con 4 bits.

#### Ejemplo:
Decimal 45 →  
4 = 0100  
5 = 0101  
Resultado: 0100 0101

---

### 3.2 Código Gray

Solo cambia **un bit** entre valores consecutivos.

#### Ejemplo:
| Decimal | Gray |
|--------|------|
| 0      | 000  |
| 1      | 001  |
| 2      | 011  |
| 3      | 010  |

#### Aplicaciones:
- Sensores
- Encoders
- Sistemas digitales con reducción de errores

---

### 3.3 ASCII

Código para representar caracteres.

#### Características:
- Usa 7 u 8 bits
- Representa letras, números y símbolos

#### Ejemplo:
- 'A' → 65 → 01000001
- '0' → 48 → 00110000

---

## 4. 🔄 Circuitos Conversores de Códigos

Permiten transformar un código en otro usando **lógica combinacional**.

### 4.1 Concepto
Un conversor recibe un código de entrada y genera otro código de salida.

---

### 4.2 Ejemplo: BCD a Gray

#### Pasos:
1. Construir tabla de verdad
2. Simplificar con mapas de Karnaugh
3. Implementar con compuertas lógicas

---

### 4.3 Ejemplo de expresión lógica

Si:
- Entradas: A, B, C, D
- Salida: G


G = A ⊕ B

#  Ejercicios Resueltos: Códigos Digitales

---

## 1. 🔢 Conversión a BCD (8421)

### 🎯 Problema:
Convertir el número decimal **27** a BCD.

### ✅ Paso 1: Separar dígitos
27 → 2 y 7

### ✅ Paso 2: Convertir cada dígito a binario (8421)

- 2 → 0010  
- 7 → 0111  

### ✅ Resultado final:

27 = 0010 0111 (BCD)
