# BC Cuentas contables multidígito

Extensión desarrollada para Microsoft Business Central. Se trata de una extensión que tiene dos funcionalidades específicas en el área contable, ampliar o reducir el número de dígitos de las cuentas auxiliares que son cargados por defecto. Cubre las necesidades las empresas y de los partners al ayudar adecuar la estructura el plan contable estándar de Microsoft Business Central. En este sentido, permite configurar el plan de cuentas en base al número de dígitos que utilice la empresa, evitando cambiar la estructura del plan de cuentas que pudiera estar utilizando antes de la sustitución por Business Central.
IMPORTANTE: Esta utilidad está pensada y diseñada para ser utilizada dentro del plan de configuración e implantación de una NUEVA EMPRESA.

# Funcionalidades:

# 1. AMPLIAR DIGITOS:
Business Central incluye una estructura de plan de cuentas en las que las cuentas auxiliares tienen 7 dígitos. 4 dígitos para definir las cuentas (3) y subcuentas (4) de un grupo determinado y 3 dígitos para definir las cuentas auxiliares. La extensión desarrollada por Neodata permite ampliar esta estructura añadiendo 0 delante de los 3 dígitos que componen cada cuenta auxiliar. Estos cambios son realizados en todas y cada una de las tablas en las que exista el campo Cuenta contable. 
Ejemplo: Queremos que nuestro número de cuenta pase de 7 dígitos a 10 dígitos. Poniendo como ejemplo a una cuenta de amortizaciones 2813001, esta utilidad transformaría el código de cuenta en 2813000001, incluyendo en este caso 3 ceros delante de los tres dígitos iniciales que componían la cuenta auxiliar.

# Procedimiento:
1.1.	Buscamos en el menú de búsqueda rápida de Business Central: "Cambiar Nº de dígito de plan de cuentas aux.".

![imagen](https://github.com/NEODATA-BUSINESS-S-L/soporte_bcextensiones/assets/129171065/58ce5b6b-e85f-43db-a8d5-9ad9cf2f5151)

1.2.	Entramos en el formulario del reporte que denominamos: "Cambiar Nº de dígito de plan de cuentas aux."
1.3.	Una vez estamos dentro de esta opción, nos pide que informemos el número de dígitos que queremos configurar para nuestras cuentas auxiliares de acuerdo con la estructura de plan de cuentas que requiere la empresa que estamos configurando. En este ejemplo informamos 10 en el campo "Dígitos de longitud de las cuentas".

![imagen](https://github.com/NEODATA-BUSINESS-S-L/soporte_bcextensiones/assets/129171065/7de09d36-07a8-48ef-81df-4f29a60a8ceb)

1.4.	Una vez hacemos clic en el botón "Aceptar", empieza el proceso de cambio de estructura, realizándose todos los cambios en todas las tablas en las que exista el campo Cuenta contable.

![imagen](https://github.com/NEODATA-BUSINESS-S-L/soporte_bcextensiones/assets/129171065/4eb01e2f-3ece-4739-9e5f-e4e8569be389)

1.5.	Tras acabar el proceso podemos ir a la página de resultados (lista de los resultados del proceso) denominada "Tabla Registros Cuentas Contables", pudiendo revisar todos los cambios que ha realizado el proceso anterior.

![imagen](https://github.com/NEODATA-BUSINESS-S-L/soporte_bcextensiones/assets/129171065/3e7a98a4-3a5d-4801-bb56-0a8cd18bfbd9)

En esta vista o página, encontramos información como:
-	El número de la cuenta inicial
-	El nuevo número de la cuenta
-	El tipo de cuenta
-	El Id del autor que hice el cambio
-	La hora de la modificación

![imagen](https://github.com/NEODATA-BUSINESS-S-L/soporte_bcextensiones/assets/129171065/8c332186-5a1e-439d-a145-f6501877422a)

El resultado en resumen es:
Número cuenta inicial: 		2813001
Número cuenta cambiada: 	2813000001

# 2. DESHACER CAMBIOS:
En caso de haber cambiado la estructura de cuentas auxiliares de forma errónea y querer volver al estado anterior, el proceso realizaría el paso contrario al reducir los dígitos de la cuenta auxiliar de los 10 a los 7 iniciales, quitando los tres ceros que hemos incluido en el proceso de ampliación.
Ejemplo: Queremos que nuestro número de cuenta pase de 10 dígitos a 7 dígitos
2.1. Buscamos la opción: “Deshacer cambios y reducir Nº de dígitos de las cuentas auxiliares”

![imagen](https://github.com/NEODATA-BUSINESS-S-L/soporte_bcextensiones/assets/129171065/06d36391-9227-4556-a512-8223abac9931)

2.2. En el campo: "Cuántos dígitos tienen las cuentas" ponemos: 10
2.3. En el campo: "Cuántos 0 quitar" ponemos: 3
2.4. Hacemos click en el botón "Aceptar".

![imagen](https://github.com/NEODATA-BUSINESS-S-L/soporte_bcextensiones/assets/129171065/4b08184c-a286-4e95-81ed-9bfe6dbce32e)

2.5. Tras acabar el proceso podemos consultar el resultado en la página "Tabla Registros Cuentas Contables"

![imagen](https://github.com/NEODATA-BUSINESS-S-L/soporte_bcextensiones/assets/129171065/1e0c762a-1fa3-402a-b0dd-ea0e341f08b5)

El resultado en la cuenta que hemos tomado como ejemplo será:
Número cuenta inicial: 		2813000001
Número cuenta cambiada: 	2813001





