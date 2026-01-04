🧮 Calculadora de Integrales Vectoriales (Numérica vs Exacta)
Este proyecto es una herramienta interactiva diseñada para el análisis de Cálculo Vectorial. 
Permite aproximar integrales dobles y triples sobre regiones estándar utilizando Sumas de Riemann de punto medio y compararlas con sus valores teóricos exactos.
🚀 Características principales
1. Soporte Multidimensional: Cálculo de integrales dobles ($\iint$) y triples ($\iiint$).
2. Sistemas de Coordenadas: Implementación de cambios de variable y Jacobianos para: a) Cartesianas (Rectángulos y Cajas). b) Polares (Discos).c) Cilíndricas (Cilindros).d) Esféricas (Esferas).
3. Visualización Avanzada: Representación gráfica de la región mediante campos vectoriales (conos) utilizando Plotly.js.
4. Análisis de Error: Cálculo automático del error relativo entre el método numérico y el valor exacto.
  
📐 Fundamento Matemático
La calculadora resuelve aproximaciones mediante la partición del volumen/área en $n^k$ subelementos. Para asegurar la precisión, el software aplica el Teorema del Cambio de Variable:

$$\iiint_V f(x,y,z) dV = \iiint_{V^*} f(g(u,v,w)) \cdot |J(u,v,w)| \, du \, dv \, dw$$

Donde $|J|$ es el determinante del Jacobiano correspondiente: 

Polares/Cilíndricas: $|J| = r$
Esféricas: $|J| = \rho^2 \sin(\phi)$

🛠️ Tecnologías utilizadas
HTML5 / CSS3: Interfaz de usuario con diseño "Dark Mode" y efectos de glassmorphism.
JavaScript (ES6+): Lógica de integración numérica y algoritmos de mapeo de coordenadas.
Plotly.js: Motor de renderizado 3D para la visualización del campo vectorial.

📖 Instrucciones de Uso
1. Seleccionar Función: Elige una función del catálogo (Ej. Potencial Cuadrático).
2. Definir Región: Selecciona el sistema de coordenadas (ej. Esféricas para una bola unitaria).
3. Ajustar Resolución: Ingresa el número de particiones por eje ($n$). A mayor $n$, menor será el error relativo.
4. Calcular: Presiona el botón para obtener el resultado numérico, el teórico y la gráfica 3D interactiva.
  
📝 Autores
Meza Santos Jose Enrique
Ocampo Crisostomo Alejandro Neftali
Sánchez Ponce Mauricio Alejandro
