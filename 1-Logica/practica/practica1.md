# Ejercicios  
 
## Uso de la Lógica de Enunciados como Lenguaje de Representación de Conocimiento (KRL).  
 
1. Representar simbólicamente las siguientes expresiones de lenguaje natural al lenguaje de la lógica de enunciados:  
 
- (a) Juan necesita un matemático o un informático.  
    p: "Juan necesita un matemático"
    q: "Juan necesita un informático"
    p ∨ q

- (b) Si Juan necesita un informático entonces necesita un matemático.  
    p: "Juan necesita un matemático"
    q: "Juan necesita un informático"
    p → q

- (c) [Duda xd] Sólo si Juan necesita un informático, Juan no necesita un matemático.  
    p: "Juan necesita un matemático"
    q: "Juan necesita un informático"
    ~p → q, en realidad mi primer pensamiento fue q → ~p pero eso significaría que si Juan necesita un informático entonces no necesita un matemático pero que Juan no necesita un matemático sólo si necesita un informático  
    

- (d) El proyecto sólo tendrá éxito si Juan contrata un informático.  
    p: "El proyecto tiene éxito"
    q: "Juan contrata un informatico"
    p → q  


- (e) Si el proyecto no tiene éxito entonces Juan no ha contratado un informático.  
    p: "El proyecto tiene éxito"
    q: "Juan contrata un informatico"
    ~p → ~q es lo mismo que hacer q → p : si Juan contrata un informático entonces el proyecto tiene éxito 


- (f) El proyecto tendrá éxito si y sólo si Juan contrata un informático.  
    p: "El proyecto tiene éxito"
    q: "Juan contrata un informatico"
    (q → p) ∧ (p → q)  
    Juan contrata unn informático entonces el proyecto tendrá éxito, y si el proyecto tiene éxito es porque Juan contrató un informático. 


- (g) Para aprobar Lógica, el alumno debe asistir a clase, desarrollar un cuaderno de prácticas aceptable y demostrar que dicho cuaderno ha sido desarrollado por él; o desarrollar un cuaderno de prácticas aceptable y aprobar el examen final.  
    p: "el alumno asiste a clase"
    q: "el alumno desarrolla un cuaderno de prácticas aceptable"
    r: "el cuaderno fue desarrollado por el alumno" 
    s: "el alumno aprueba el examen final"
    t: "aprobar lógica"
    t → (((p∧q)∧r) ∨ (q∧s))

- (h) El alumno puede asistir a clase u optar por un examen libre.  
    p: "Alumno asiste a clase"
    q: "Alumno opta por rendir examen libre"
    (p ∨ q)


- (i) Si x es un número racional e y es un entero, entonces z no es real.  
    p: "x es un número racional"
    q: "y es un número entero"
    r: "z es un número real"
    (p∧q) → r

- (j) La suma de dos números es par si y sólo si los dos números son pares o los dos números son impares.  
    p: "dos números son pares"
    q: "dos números son impares"
    r: "la suma de dos números es par"
    r ↔ (p∨q)


## Valores de verdad y tablas de verdad.  
 
2. Decimos que una fbf del Cálculo de Enunciados es satisfactible si y sólo si existe al menos una asignación de valores de verdad para las letras de proposición en la fbf que la hace verdadera. Verificar si las siguientes fbfs son satisfactibles o no.  
  
i- p → q 
ii- p → p 
iii- p ↔ r  
iv- r ∨ s 
v- s ↔ ¬q 
vi- s ∧ ¬s no es satisfactible pues se tendría que cumplir que ambas sean verdaderas pero si s = v, entonces ~s = f lo que dejaría a la fórmula como F

3. Decimos que un conjunto   Γ de fbfs del Cálculo de Enunciados  es satisfactible  si y só lo si existe al menos una asignación de valores de verdad para las letras de proposición que hace verdadera a cada fbf. Determinar si los siguientes conjuntos de fbfs son o no satisfactibles . Fundamentar.  
 
i-   Γ = {p → q, p ↔ q, r ∨ s, s ↔ ¬q} 
ii-  Γ  = {¬p ∨ ¬q, p ∨ q, p ∨ ¬q, ¬p ∨ q} 
 

## Formas argumentativas.  
4. Determinar, si es posible, cuáles formas argumentativas son válidas y cuáles no. Fundamentar.  
 
p → q   r      q ∨ ¬p   p → q   p ↔ q 
t ∨ ¬q  p ∨ (q → r)    r → p    r ∨ ¬q   q ∨ p 
s ∧ p  p ∨ ¬q   r → q    s ∧ p   q ∧ ¬p 
s ∧ t     s ∧ ¬r 
 
## Argumentaciones.  
 
5. Dada la siguiente información, representarla simbólicamente; Si el unicornio es mìtico, entonces 
es inmortal, pero si no es mítico, entonces es un mamí fero mortal. Si el unicornio es o inmortal  o un 
mamífero, entonces tiene un cuerno. El unicornio es mágico sí tiene un cuerno.   
Teniendo la información previa como premisas, determinar si es posible concluir:  
 
a- ¿El unicornio es mìtico?. Fundamentar.  
b- ¿El unicornio no es mìtico?. Fundamentar.  
c- ¿El unicornio es mágico?. Fundamentar.  

6. Simbolizar: Se sabe que: La página web tiene un error o el examen de álgebra no es el 2 de julio. Si 
el examen de álgebra es el 2 de julio entonces la pá gina web tiene un error. El examen de álgebra es 
el 14 de julio si y sólo si la página web tiene un error y el período de exámenes no termina el 10 de 
julio.  
 
Teniendo en cuenta que el período de exámenes termina el 10 de julio y que la página web tiene un 
error, determinar la verdad o falsedad de las siguientes conclusiones:  
 
(a) El examen de álgebra es el 2 de julio.  
(b) Si la página web no tiene un error entonces el examen de álgebra es el 14 de julio.  
 
7. Se tienen las siguientes premisas: Si Juan tiene suerte y llueve entonces estudia. Juan aprobará si y 
sólo si estudia o tiene suerte. Si Juan no tiene suerte entonces no llueve. Sabiendo que llueve, 
responder lo siguiente : 
(a)¿Aprobará  Juan?. Fundamentar.  
(b) ¿Tendrá suerte Juan?. Fundamentar.  
 
8. Guillermo está planeando una reunión en su casa pero los del grupo nos llevamos mal entre 
nosotros. Si va Hugo, vamos a estar mal si yo estoy ahí. Yo voy sólo si Lucía va. Lucía no va a ir a 
menos que Julieta vaya.  
Modelizar y determinar formalmente: ¿Es posible que en lo de Guillermo nos juntemos al menos 
tres de modo que estemos bien? ¿Es posible que vayamos los  cinco y estemos bien?  Fundamentar.  
 
9. Simbolizar usando al Cálculo de Enunciados como KRL  e investigar la validez de la argumentación 
siguiente: Los nitratos se forman del nitrógeno atmosférico libre o de las proteínas descompuestas 
por el suelo. Cuando los nitratos se forman del nitrógeno atmosférico libre, entonces ese proceso de 
formación de nitratos se denomina fijación del nitrógeno y no incluye liberación de amoníaco de las 
proteínas descompuestas. Por lo tanto, cuando no se advierte la presencia de amoníaco liberado, 
ocurre que los nitratos no se formaron de las proteínas descompuestas por el suelo.  
 

---
# Notas 

**Condición suficiente**: “Si …, entonces …”
Decir: 𝑝 → 𝑞 significa que p es suficiente para q.
👉 Cada vez que hay p, seguro hay q.

**Condición necesaria**: “Sólo si …”
Decir: 𝑝 → 𝑞 significa que q es condición necesaria para p.
👉 Para que se cumpla p, q debe estar sí o sí.