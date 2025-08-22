# LeIA - Teoría - Clase 1: Lógica proposicional

> Enlace: https://drive.google.com/file/d/1X-5OZ_j4Y-FMt0Vx1XGERSMa6Q3LSYbS/view 

La lógica permite obtener y justificar conclusiones a partir de verdades supuestas (premisas).

Premisas --(Mecanismo de razonamiento)--> Conclusiones 

Estos se expresan mediante un lenguaje formal: lenguaje de la lógica para representar el conocimiento. 
**Razonamiento**: encadenamiento de enunciados formado por premisas y conclusiones. 

> El lenguaje tiene SINTAXIS y SEMÁNTICA 


## Lenguaje de la lógica
La lógica de **enunciado** o proposicional representa frases. 
Las conectivas más comunes y los símbolos que emplearemos para denotarlas son los siguientes:

| Conectiva         | Símbolo   | Ejemplo      | Significado                  |
|-------------------|-----------|--------------|------------------------------|
| Negación          | ~         | ~A           | No A                         |
| Conjunción        | ∧         | A ∧ B        | A y B                        |
| Disyunción        | ∨         | A ∨ B        | A o B                        |
| Condicional       | →         | A → B        | Si A entonces B              |
| Bicondicional     | ↔         | A ↔ B        | A si y solo si B             |


### Sintaxis: el lenguaje simbólico de la lógica 
El lenguaje simbólico consta de un conjunto de símbolos _primitivos_ (el **alfabeto** o vocabulario) y un conjunto de _reglas_ de formación (la **gramática**) que nos dice cómo construir fórmulas bien formadas a partir de los símbolos primitivos. 

#### Alfabeto
Conjunto de símbolos que pertenecen al lenguaje del sistema. Si L es el nombre del sistema de lógica proposicional, entonces el alfabeto de L consiste en: 
- Una cantidad finita pero arbitrariamente grande de variables proposicionales. Uso de la letra p, luego q, etc. 
- Un conjunto de operadores lógicos o conectivas: ~,∧,∨,→,↔
- Dos signos de puntuación para desambiguar ciertas expresiones (paréntesis). 

#### Gramática 
Determina qué combinaciones de símbolos pertenecen al lenguaje del sistema. Esto se logra mediante una gramática formal que consiste en un conjunto de reglas que definen recursivamente las cadenas de caracteres que pertenecen al lenguaje. A las cadenas de caracteres construidas según estas reglas se las llama _fórmulas bien formadas_. 
Dado un sistema L, las seglas son: 
i. las variables de enunciado son formas enunciativas, es decir, p, q. 
ii. si A y B son formas enunciativas de L entonces también lo son otras fórmulas bien formadas usando las conectivas (**llevan paréntesis**, son parte del alfabeto). 
ii. Solo las expresiones que pueden ser generadas mediante las cláusulas i y ii en un _número finito de pasos_ son formas enunciativas de L.

> Denotaremos con letras minúsculas p, q, r, ..., a las variables que designan enunciados simples arbitrarios. Nótese la distinción entre los usos de las letras p, q, r, …, y las letras A, B, C, ... Las primeras son variables que pueden ser sustituidas por enunciados simples particulares. Las últimas son meras etiquetas que designan enunciados en general.

### Semántica: interpretación y satisfacción
Como todo enunciado simple es verdadero o falso, una variable de enunciado tomará uno u otro valor de verdad: V (verdadero) o F (falso). La verdad o falsedad de un enunciado compuesto depende de la verdad o falsedad de los enunciados simples que lo constituyen, y de la forma en que están conectados. 

#### Tablas de verdad

**Negación (~)**
| p | ~p |
|---|----|
| V | F  |
| F | V  |

**Conjunción (∧)**
| p | q | p ∧ q |
|---|---|-------|
| V | V |   V   |
| V | F |   F   |
| F | V |   F   |
| F | F |   F   |

**Disyunción (∨)**
| p | q | p ∨ q |
|---|---|-------|
| V | V |   V   |
| V | F |   V   |
| F | V |   V   |
| F | F |   F   |

**Condicional (→)**
| p | q | p → q |
|---|---|-------|
| V | V |   V   |
| V | F |   F   |
| F | V |   V   |
| F | F |   V   |

**Bicondicional (↔)**
| p | q | p ↔ q |
|---|---|-------|
| V | V |   V   |
| V | F |   F   |
| F | V |   F   |
| F | F |   V   |

#### Tablas de verdad para enunciados compuestos 
El valor de verdad de un enunciado compuesto depende del valor de verdad de los enunciados simples (atómicos).

#### Interpretación
Es una función que relaciona los elementos del dominios sintáctico y semántico de la lógica considerada. 
Minuto 53