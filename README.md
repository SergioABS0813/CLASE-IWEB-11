# CLASE-IWEB-11

## Compilar Proyecto bajado desde la nube
No podemos compilar el proyecto bajado de Github.

![image](https://github.com/SergioABS0813/CLASE-IWEB-11/assets/134556600/9797ba42-a0ad-4125-a4c3-df45d362dfe1)

1)
![image](https://github.com/SergioABS0813/CLASE-IWEB-11/assets/134556600/58a15581-6b62-4d1e-a639-e638cbe5c958)

2)
![image](https://github.com/SergioABS0813/CLASE-IWEB-11/assets/134556600/dbfacc32-02b5-418c-b18f-9c46850e478c)

3) Nos damos cuenta que falta el .jar que sirve para compilar el proyecto
![image](https://github.com/SergioABS0813/CLASE-IWEB-11/assets/134556600/1fbec5fc-a0a2-489e-be58-19869c5ce55b)

4) Nos aparecerán 2 opciones, damos clic a "warexploded". Luego, cambiamos el nombre de "warexploded" si deseamos y luego "aplly" "ok"

Resultado:

![image](https://github.com/SergioABS0813/CLASE-IWEB-11/assets/134556600/5852c07a-8a5f-4175-b04f-a907822cd83f)

## Crear clase BaseDao
Esta clase solo realiza conexión con la base de Datos y permite generalizar y usarla en cualquier clase Dao y métodos dentro de cada Dao. Para no estar copiando y pegando a cada rato el Driver o los parámetros de conexión. 

Así, el método de conexión, lo podrán usar todos los hijos de BaseDao por herencia.

![image](https://github.com/SergioABS0813/CLASE-IWEB-11/assets/134556600/640e2167-8b09-4b92-9742-555ca9a63f3b)

Cabe resaltar que podemos trabajar con varias bases de datos, solo hacemos otro método dentro de BaseDao.

## Clases Abstractas
Son clases que no necesitamos instanciar, por ejemplo, HTTPServlet o DaoBase.

Vemos que DaoBase es abstracta:

![image](https://github.com/SergioABS0813/CLASE-IWEB-11/assets/134556600/640e2167-8b09-4b92-9742-555ca9a63f3b)

## Métodos Abstractos
Son métodos que se designan en las clases Padre para que las clases hijo deban sí o sí implementarla en la propia clase.

Ejemplo de vida real: Persona es la clase Padre, Alumno y Profesor son clases hijos de Persona, entonces colocamos el método de "estudiar" en persona y de seguro que el alumno y el profesor estudian de forma diferente, pero ambos sí o sí tienen que estudiar.

Implementamos métodos comer y estudiar abstractos.

Luego implementamos "saltar" como método.

![image](https://github.com/SergioABS0813/CLASE-IWEB-11/assets/134556600/8bdc2669-1146-411f-b31b-286d37540286)

En profesor: Es necesario colocar ambos métodos abstractos, pero para saltar no es necesario

![image](https://github.com/SergioABS0813/CLASE-IWEB-11/assets/134556600/07edfb42-73cf-45c2-b9ed-0f41f31f81a8)

## Razonamiento sobre Métodos y Clases Abstractas (Ejemplo Persona, Profesor, Alumno, Alumno Teleco y Alumno Electrónico)

![image](https://github.com/SergioABS0813/CLASE-IWEB-11/assets/134556600/357b2cef-4caa-4aad-90a1-3ade8a002a1d)

![image](https://github.com/SergioABS0813/CLASE-IWEB-11/assets/134556600/e97001a0-a107-471e-9c61-8bf0b5f71cae)

## Modificación del listado con INNER o LEFT JOIN (Aprovechamiento de Beans)

Queremos saber a qué nombres de departamento y empleado hacen referencia el managerID y el departmentID

Migramos y empleamos Beans como atributos y luego generamos Getters y Setters de nuevo:

![image](https://github.com/SergioABS0813/CLASE-IWEB-11/assets/134556600/60697abd-506b-47c0-8c26-065c0392af59)


Empleamos este Query que concatena tablas en una sola comparando los valores de los atributos:

![image](https://github.com/SergioABS0813/CLASE-IWEB-11/assets/134556600/733531d5-079a-4579-9769-78267d47cb9e)

Colocamos el Query. El método fetch sacará la info necesaria y los pondrá en cada empleado para que en este método que vemos solo se listen. Ahora, sacaremos información pero a través de Beans

![image](https://github.com/SergioABS0813/CLASE-IWEB-11/assets/134556600/3c81dadb-1861-4b17-96eb-5b5aa0097083)

Cambios en el Fetch ahora teniendo como atributo a los Beans:

![image](https://github.com/SergioABS0813/CLASE-IWEB-11/assets/134556600/9cdf9e8a-c120-4573-be92-d7cecbee156a)

Referencia de "e" y "m" en el Query por esta tabla:

![image](https://github.com/SergioABS0813/CLASE-IWEB-11/assets/134556600/8fa8918b-483c-4d93-b5b1-9cfc3557b53e)





## Arreglamos de capa en capa ()
















