# Bono de Programación — Problemas 2 y 3  

Estudiante: Javier David Nuñez Robles  
Materia: Matemáticas Discretas I  
Universidad: Universidad Nacional de Colombia  
Docente: Jhoan Sebastian Tenjo García

\---

## Estructura del Proyecto  
`main.py\`: Archivo fuente principal en Python con las funciones, validaciones de errores y casos de prueba.  
`docs/evidencias.txt\`: Registro de la salida generada por la consola al ejecutar las pruebas.

\---

## Problemas Seleccionados

### Problema 2. Calculadora General de Combinaciones  

Descripción: Calcula el número de formas de seleccionar $r$ elementos de un conjunto de $n$ objetos donde el orden de selección    no importa.
  
Fórmula: $$\\binom{n}{r} \= \\frac{n\!}{r\!(n-r)\!}$$  

Eficiencia: Implementado en tiempo $\\mathcal{O}(\\min(r, n-r))$ mediante el uso estratégico de la identidad de simetría $\\binom{n}{r} \= \\binom{n}{n-r}$, evitando desbordamientos de memoria al prescindir del cálculo aislado de factoriales masivos.




### Problema 3. Conteo de Cadenas Binarias con Restricciones  

Descripción: Determina la cantidad total de cadenas binarias de longitud $n$ bajo criterios dinámicos ingresados por el usuario.  

Principios Combinatorios:

Sin restricciones: Regla del producto ($2^n$).  

Exactamente $k$ unos: Coeficiente binomial $\\binom{n}{k}$.  

A lo sumo $k$ unos: Sumatoria acumulada $\\sum\_{i=0}^{k} \\binom{n}{i}$.  

Al menos $k$ unos: Sumatoria acumulada $\\sum\_{i=k}^{n} \\binom{n}{i}$.  


Eficiencia: Complejidad temporal lineal de $\\mathcal{O}(n)$ en los peores escenarios (sumatorias completas), garantizando respuestas inmediatas.

\---

## Instrucciones de Ejecución

Siga estos pasos para ejecutar el proyecto en su computadora:

1. Requisitos Previos
Tener instalado Python 3.x. Puede verificarlo ejecutando:

```bash
#```bash
python --version
```

2. Clonar el Repositorio
Descargue el proyecto en su entorno local:

Bash
git clone https://github.com/TU_USUARIO/bono-programacion-discretas.git
(Cambie TU_USUARIO por su nombre real de GitHub).

3. Navegar a la Carpeta
Entre al directorio del proyecto:
Bash
cd bono-programacion-discretas


4. Ejecutar el Programa
Corra las funciones de conteo combinatorio y las pruebas automatizadas con:

Bash
python main.py
