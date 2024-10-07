# Extortion_Peru
Este repositorio cuenta con información sobre las bases de datos de mi tesis de licenciatura, así como la elaboración del apartado cuantitativo de la misma.
El tema de investigación a analizar es acerca de qué factores permitieron el aumento del número de delitos por extorsión a nivel nacional. Para esto, se toma en cuenta múltiples variables que se encuentran en el archivo **datafinal.csv**
# Variables
Las variables en cuestión son:
## Variables independientes
**UBICACION**= esta variable con tiene los distritos del Perú en un formato concatenado en el que se agrupa el departamento y la provincia donde se encuentra ubicado el distrito. De este modo, se evita confusiones al momento de realizar la unión de variables.
**num_comisarias**= Esta variable contiene el numero de las comisarias a nivel nacional en cada distrito de Perú entre los años 2019 y 2021.
**personal**= contiene el número de efectivos policiales en un determinado distrito.
**area_com**= es el area ocupada por comisarias en cada distrito
**old_com** = es la suma de la antigüedad de cada comisaria por distrito
**com_internet** = es el numero de comisarías a nivel nacional que cuentan con internet por distrito
**nreu_codisec** = devuelve el número de reuniones del Comité Distrital de Seguridad Ciudadana realizado durante el año en las que participaron los comisarios.
**juntas**= es el número de juntas vecinales por distrito a nivel nacional
**per_juntas** = es el número de personas que participa en la junta vecinal por distrito
**redes** = es el numero de redes de cooperantes por distrito encargados de brindar información acerca de hechos delictivos a los comisarios
**per_redes**= número de personas por distritos que conforman las redes de cooperantes
**n_patru** = es el numero de acciones de patrullaje por día que se realiza por distrito a nivel nacional
**n_pat_int** =  es el número de acciones de patrullaje integrado por día que realizan serenazgo y las comisarias en cada distrito
**serenazgos**= es el numero de serenazgos según distrito
**n_vehi**= numero de vehículos de serenazgo por cada distrito
**conf_pnp** = es el índice de confianza en la policía
**conf_muni** = es el indice de confianza en la municipalidad
**conf_pj**= es el indice de confianza en el Poder Judicial por parte de la poblacion
**conf_mpfn** = es el indice de confianza en el Ministerio Público Fiscalia de la Nacion
**ANIO** = es el año en el que se registra la información. Abarca desde 2019 hasta 2020
## Variable dependiente
**denuncias** = es el número de denuncias por extorsión ocurrido en cada distrito a nivel nacional
