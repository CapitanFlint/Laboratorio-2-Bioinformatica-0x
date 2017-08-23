# Laboratorio 2 Bioinformática 23/08/2017

# Bruno Romero

------

# Parte 1 : Colectar genes homólogos

------

#### ¿Qué función cumple el gen SRY?

__R:__

+ `El gen codifica para una proteína que es un factor de transcripción, denominado TDF (testis-determining factor), el cual participa en la determinación del sexo masculino en humanos y otras especies que poseen ortólogos.`


#### ¿Cuántos genes ortólogos están anotados en esa base de datos?

__R:__

+ `En la base de datos se detallan 26 secuencias ortólogas.` [1]


# Parte 2: Alineamiento múltiple

------

#### ¿Qué es el EMBL-EBI?

__R:__

+ `El EMBL-EBI es el Instituto de bioinformática Europeo. Sus objetivos principales es apoyar a la investigación científica entregando y otorgando un servicio de alojamiento de datos y de comparación de los mismos. `

> "EMBL-EBI is international, innovative and interdisciplinary, and a champion of open data in the life sciences"


#### ¿Cuántos tipos de alienamiento múltiple se pueden realizar en EMBL-EBI?

__R:__

+ `Existen dos generales: Multiple Sequence Alignment (MSA) y Pairwise Sequence Alignment, en donde cada uno posee subtipos correspondientes a cada programa y desarrollador bioinformático que poseen distintos enfoques y funcionalidades. `


#### ¿Cuál es el programa que ellos ofrecen que funciona mejor para secuencias de proteínas?

__R:__

+ `Clustal Omega [2], MUSCLE [3] y Align UniProt [4].`


#### ¿Qué otros tipo de herramientas ofrece EMBL-EBI?

__R:__

+ `Posee muchísimas otras herramientas [5] `


#### ¿Cuál es el costo de abrir un gap?

__R:__

+ `El costo de abrir un gap es de 1.53 [6] `

#### ¿Cuál es el costo de extender un gap?

__R:__

+ `El costo de extender un gap es de 0.123 `


#### ¿Cuál es la longitud total del alineamiento?

__R:__


+ `El alineamiento posee 1932 columnas en el fragmento consensus. `

#### ¿Cuál es la especie cuyo gen SRY está más relacionado con el gen SRY de humanos?

__R:__

+ `La especie que posee el mRNA más cercano a la especie humana es Pan troglodytes. `


#### ¿Cuál es el más lejano?

__R:__

+ `La especie más lejana es Pteropus alecto, ya que posee la puntuación más alta (0.12288) `


#### ¿Cuál es la especie cuyo gen SRY es más cercana a la del burro?

__R:__

+ `La especie más cercana al mRNA del burro es Equus przewalskii. `


#### ¿Cómo esperas que sea el alineamiento si el costo de abrir un gap aumenta? ¿Y si disminuye?

__R:__

+ `Si el puntaje de penalización de abrir gaps aumenta, entonces el programa tenderá a tener una menor cantidad de gaps pero con una mayor extensión cada uno.` 


#### ¿Cómo esperas que sea el alineamiento si el costo de extender un gap aumenta? ¿Y si disminuye?

__R:__


+ `Si el puntaje de extender un gap aumenta, entonces el programa va a tender a favorecer muchos gaps de muy corta longitud. `


#### ¿Cuál fue el efecto de aumentar el costo de abrir un gap en la longitud total del alineamiento? prueba lo mismo pero esta vez disminuyendo al mínimo el costo de extender un gap. Describe cómo cambia el alineamiento


__R:__

+ `Al aumentar de 1.53 a 2.00, la longitud total del consensus fue la misma que en 1.53. Esto se deba probablemente a que los dominios que conforman a la proteína homóloga estén conservados evolutivamente (además de ser relativamente corta). Para el valor '0,1' en extender gap, el resultado fue que la longitud total del fragmento consensus disminuyó a 1907 (vs el 1932). Esto es porque los gaps que se abrieron son de menor longitud. `

# Parte 3: Diseño de partidores

------





### Secuencia mRNA Gen SRY humano https://www.ncbi.nlm.nih.gov/nuccore/NM_003140.2



# Bibliografía

[1] https://www.ncbi.nlm.nih.gov/gene/?Term=ortholog_gene_6736[group]
[2] http://www.ebi.ac.uk/Tools/msa/clustalo/
[3] http://www.ebi.ac.uk/Tools/msa/muscle/
[4] http://www.uniprot.org/align/
[5] http://www.ebi.ac.uk/services/all
[6] http://www.ebi.ac.uk/Tools/msa/mafft/
