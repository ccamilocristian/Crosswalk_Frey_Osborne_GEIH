# Crosswalk Frey & Osborne- GEIH

Objetivo: Realizar la correlativa del código SOC-10 (Standard Occupational Classification) de O*NET[^1] a 6 dígitos con código CNO-70 (Clasificación Nacional de Ocupaciones) del SENA a dos dígitos, para empalmar resultados de Frey &Osborne (2013) a los datos colombianos GEIH.

Metodología:
1. Wojciech Hardy del Instituto de investigación estructural, en conjunto con la Facultad de Economía de la Universidad de Warsaw, desarrollaron una correlativa para el SOC-10 a 6 dígitos con el CIUO-08 a 4 dígitos (Clasificación Internacional Uniforme de Ocupaciones) [^2].
2. Por otro lado, la Organización Internacional del Trabajo[^3] desarrolló una correlativa del CIUO-08 y el CIUO-88, ambas a 4 dígitos. Basado en esta correspondencia, se cruzó ésta con la base del inciso número 1, arrojando una base insumo de la forma SOC-10 y CIUO-88.
3. Transcribir a una base de datos la correlativa realizada por DANE del código CIUO-88 de 4 dígitos a la CNO-70 a cuatro dígitos[^4].
4. Agrupar el código CNO-70 a dos dígitos y relacionar el código CIUO-88 a 4 dígitos correspondiente. En este punto, se realiza una limpieza de la agrupación en donde se eliminen duplicados y ocupaciones del CIUO-88 a cuatro dígitos que no corresponden a la subcategoría de CNO-70 a los dos dígitos que usa el DANE en la GEIH.
5. Cruzar la base del inciso número dos por la llave CIUO-88 con la base del inciso anterior para obtener una correlativa del código CNO-70 a dos dígitos con el SOC-10 a 6 dígitos.
6. Cruzar la base de probabilidades de riesgo de automatización del paper de Frey & Osborne (2013) con la base del inciso anterior, por la llave SOC-10 a 6 dígitos. Luego, agrupar a nivel de CNO-70 y dejar el promedio de probabilidades relacionadas a los códigos SOC-10 en la correlativa del punto 5.
7. Cruzar la base insumo de la GEIH de Colombia para los años de referencia (la llave es la variable OFICIO) y la base del punto 6 a nivel de CON-70 (la llave es el CNO-70), para traer la probabilidad de riesgo de automatización para el caso colombiano dato los datos de Frey & Osborne.


[^1] Occupational Information Network
[^2] Hardy, W. (2016). IBS. Obtenido de Occupation classifications crosswalks – from O*NET-SOC to ISCO: https://ibs.org.pl/en/resources/occupation-classifications-crosswalks-from-onet-soc-to-isco/
[^3] OIT. (2008). Estructura de la CIUO-08 y concordancias previas con la CIUO-88. Obtenido de OIT: https://www.ilo.org/public/spanish/bureau/stat/isco/isco08/index.htm
[^4] DANE (2005). Clasificación Internacional Uniforme de Ocupaciones Adaptada para Colombia CIUO-88 A. C. Bogotá D.C.: DANE