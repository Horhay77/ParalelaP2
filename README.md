Práctica MPI: Paralelización de código
=================

| Autores |
|-------|
|Lucía Gil Román|
|Jorge Hernández de Benito|

# Pasos tomados

En una primera aproximación al problema se tomaron las siguientes medidas:
- División del mapa de forma equitativa entre los procesos mediante el reparto de las filas.
- Creación de un tipo de dato derivado (`MPI_Datatype`) que almacena la antena que cada proceso cree que ha de ser colocada dentro de la región en la que opera.
- Creación de una operación de reducción (`MPI_Op`) de búsqueda de mejor antena.

# Pasos futuros

Se consideran realizar las siguientes mejoras:
- Dado que las máquinas sobre las que ejecutamos el código paralelo no tienen las mismas características, se busca desbalancear la carga de trabajo en función de la eficiencia que proporcionan.

