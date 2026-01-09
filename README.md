🧮 Calculadora de Integrales Vectoriales (Numérica vs Exacta)

Este proyecto es una herramienta web interactiva diseñada para el aprendizaje y validación del Cálculo Vectorial. Permite aproximar integrales dobles ($\iint$) y triples ($\iiint$) sobre diversas geometrías espaciales utilizando Sumas de Riemann de punto medio, comparándolas en tiempo real con sus valores teóricos exactos y validaciones externas.

🚀 Características Avanzadas

1. Motor de Expresiones Dinámicas: Gracias a la integración con Math.js, el usuario puede escribir sus propias funciones $f(x, y, z)$ utilizando sintaxis matemática estándar.

2. Sistemas de Coordenadas y Jacobianos: Implementación automática de cambios de variable para:

   a) Cartesianas: Rectángulos ($[-1,1] \times [-1,1]$) y Cajas.

   b) Polares/Cilíndricas: Discos y volúmenes cilíndricos ($|J| = r$).

   c) Esféricas: Regiones esféricas completas ($|J| = \rho^2 \sin(\phi)$).

3. Visualización Vectorial 3D: Renderizado interactivo mediante Plotly.js que proyecta la magnitud de la función como un campo de conos en el espacio tridimensional.

4. Validación Externa (Wolfram|Alpha): Un botón inteligente genera automáticamente la sintaxis de la integral (incluyendo límites y coordenadas) y la envía a Wolfram|Alpha para una validación experta.
  
📐 Fundamento Matemático

El software divide el dominio en $n^k$ sub-elementos (donde $k$ es la dimensión). La aproximación se basa en evaluar la función en el centro de cada celda para mejorar la convergencia:

$$\iiint_V f(x,y,z) dV = \iiint_{V^*} f(g(u,v,w)) \cdot |J(u,v,w)| \, du \, dv \, dw$$

Donde $|J|$ es el determinante del Jacobiano correspondiente: 

Polares/Cilíndricas: $|J| = r$

Esféricas: $|J| = \rho^2 \sin(\phi)$

🛠️ Tecnologías Utilizadas

HTML5 / CSS3: Interfaz con diseño Dark Mode y efectos de Glassmorphism para una estética moderna.

JavaScript (ES6+): Algoritmos de integración numérica y lógica de mapeo.

Math.js: Parser de expresiones matemáticas para evaluar funciones personalizadas en tiempo real.

Plotly.js: Motor de renderizado 3D para el campo vectorial.

📖 Instrucciones de Uso

1. Definir Función: Selecciona una función predefinida o elige "Escribir propia función" e ingresa expresiones como sin(x) * exp(-y^2).
<img width="844" height="315" alt="image" src="https://github.com/user-attachments/assets/d68c61cf-8c12-445e-835d-2ccc47530940" />


2. Seleccionar Región: Elige la geometría de integración (Caja, Esfera, Cilindro, etc.).
<img width="842" height="294" alt="image" src="https://github.com/user-attachments/assets/509ef74c-8928-4cc4-88e7-eb87f6d9b102" />


3. Ajustar Resolución ($n$): Define la densidad de la malla.
      NOTA: Valores de $n$ entre 15 y 25 ofrecen el mejor balance entre precisión y velocidad.
   <img width="866" height="127" alt="image" src="https://github.com/user-attachments/assets/20a09df7-82ec-4319-9e27-97816c23ef4a" />


4. Generar e Integrar: Observa la aproximación numérica, el error relativo y la gráfica. Usa el botón de Wolfram|Alpha para verificar el resultado analítico.
<img width="875" height="485" alt="image" src="https://github.com/user-attachments/assets/69b7c77a-9f72-4016-bc81-4a0446f21ccf" />
  
📝 Autores

Meza Santos Jose Enrique

Ocampo Crisostomo Alejandro Neftali

Sánchez Ponce Mauricio Alejandro
