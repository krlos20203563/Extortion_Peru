# Extortion_Peru
Este repositorio cuenta con información sobre las bases de datos de mi tesis de licenciatura, así como la elaboración del apartado cuantitativo de la misma.
El tema de investigación a analizar es acerca de qué factores permitieron el aumento del número de delitos por extorsión a nivel nacional. Para esto, se toma en cuenta múltiples variables que se encuentran en el archivo **datafinal.csv**
La presentación de dicho proyecto se encuentra en este enlace: https://krlos20203563.github.io/Extortion_Peru/
# Variables
Las variables en cuestión son:
## Variables independientes

- **UBICACION**= esta variable con tiene los distritos del Perú en un formato concatenado en el que se agrupa el departamento y la provincia donde se encuentra ubicado el distrito. De este modo, se evita confusiones al momento de realizar la unión de variables.

- **num_comisarias**= Esta variable contiene el numero de las comisarias a nivel nacional en cada distrito de Perú entre los años 2019 y 2021.

- **personal**= contiene el número de efectivos policiales en un determinado distrito.

- **area_com**= es el area ocupada por comisarias en cada distrito.

- **old_com** = es la suma de la antigüedad de cada comisaria por distrito.

- **com_internet** = es el numero de comisarías a nivel nacional que cuentan con internet por distrito.

- **nreu_codisec** = devuelve el número de reuniones del Comité Distrital de Seguridad Ciudadana realizado durante el año en las que participaron los comisarios.

- **juntas**= es el número de juntas vecinales por distrito a nivel nacional.

- **per_juntas** = es el número de personas que participa en la junta vecinal por distrito.

- **redes** = es el numero de redes de cooperantes por distrito encargados de brindar información acerca de hechos delictivos a los comisarios.

- **per_redes**= número de personas por distritos que conforman las redes de cooperantes.

- **n_patru** = es el numero de acciones de patrullaje por día que se realiza por distrito a nivel nacional.

- **n_pat_int** =  es el número de acciones de patrullaje integrado por día que realizan serenazgo y las comisarias en cada distrito.

- **serenazgos**= es el numero de serenazgos según distrito.

- **n_vehi**= numero de vehículos de serenazgo por cada distrito.

- **conf_pnp** = es el índice de confianza en la policía.

- **conf_muni** = es el indice de confianza en la municipalidad.

- **conf_pj**= es el indice de confianza en el Poder Judicial por parte de la poblacion.

- **conf_mpfn** = es el indice de confianza en el Ministerio Público Fiscalia de la Nacion.

- **ANIO** = es el año en el que se registra la información. Abarca desde 2019 hasta 2020.

## Variable dependiente

- **denuncias** = es el número de denuncias por extorsión ocurrido en cada distrito a nivel nacional.

# Metodología

Se extrajo variables de múltiples bases de datos que registran información sobre seguridad ciudadana a nivel nacional. estas son:

- **SIUP**: Este es el Sistema de Información de Unidades Policiales. Contiene información acerca de las comisarias a nivel nacional, así como el personal y diversas otras variables. Se compone de seis cuestionarios. El cuestionario 100 contiene informacion sobre el personal policial. El cuestionario 200 acerca de la infraestructura de las comisarias. El cuestionario 300 contiene información acerca del equipamiento policial según cada comsiaría. El 400 y el 500 son cuestionarios sobre el mantenimiento del equipamiento y la infraestructura, respectivamente. Por último, el cuestionario 600 contiene información sobre acciones de prevención comunitaria y articulación interinstitucional.
- **ENAPRES**: Esta es la Encuesta Nacional de Programas Presupuestales. Se realiza por parte del INEI en colaboración con el MEF para así realizar asignaciones presupuestarias según el sector. De esta base de extrajo información acerca de la confianza en la policía y demás instituciones encargadas de la seguridad ciudadana.
- **RENAMU**: es el Registro Nacional de Municipalidades. Cuenta con información según alcaldía de distrito acerca de la operatividad de la municipalidad. De aquí se extrajo información sobre el serenazgo y su equipamiento.
- **SIDPOL**: Este es el Sistema de Registro y Control de Denuncias Policiales. Cuenta con información sobre todos los delitos denunciados a nivel nacional. En el Observatorio Nacional de Seguridad Ciudadana se puede encontrar información georreferenciada de las denuncias realizadas. De aquí se extrajo la variable del número de denuncias de casos por extorsión.

Para poder analizar dichas bases de datos se utilizará un método de regresiones poisson y binomial negativa debido a que la variable dependiente es de conteo
