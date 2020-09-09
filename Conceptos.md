# Conceptos

Explicación Clases
https://gustavodohara.com/blogangular/clases-en-typescript/

# ############################################
# 4. DATA BINDING // Enlace de datos
# ############################################

# 4.1 Interpolación 
        {{ propiedad/objeto/expresión/metodo }}
# 4.2 Property binding / Enlaza valores de la fuente de datos a la vista.
        [ atributodelelementoHTML ] = “ expresión “

# 4.3 End bindign / one way / Desde la vista hasta la fuente de datos.
        evento=”nombreMetodo()”;

# 4.3 Two way binding / Enlazan datos de la vista a la fuente de datos y viciversa.
        [( directiva )] = “nombredelapropiedad”

# ############################################
# 5 DIRECTIVAS
# ############################################

        - Componentes
        - De atributos / Ng / Modifican el comportamiento de un elemento
        - Estructurales / * / Alteran el layout del elmento, adding, deleting or replacing
# 5.1 ngIf / Implementa estructuras if / Se condiona que el elmento Html se muestre o no en funcón de que se cumpla la expresión que difine. Normalemente una propiedad o método.
        *ngIf=”expresión/propiedad/metodo” 
        *ngIf="nombre; else desactivado"

# 5.2 ngStyle / Estable de manera dinámica los estilos de un elemento html en función de la expresión asociada.
        [ngStyle]=”{ expresión/propiedad/método }"

# 5.3 ngClass / Estable de forma dinámica las clases de un elemtno HTML
        [ngClass]="'first second'"

# 5.4 ngFor / Para realizar iteraciones y mostrar listados en pantalla. 
        *ngFor=”let objeto/propiedad of objetos/propiedades”  


# 5.5 ngSwitch 
# 5.6 Directivas propias
        ng generate directive              


# ############################################
# 6 PIPES
# ############################################

        {{ dato | nombredelpipe:’opciones’ }}

# 6.1 Pipe date
        Sevilla, {{ hoy | date:'d/M/y H:m'}}</p>
# 6.2 Pipe uppercase and lowercase
        {{ ciudad | uppercase}}
        {{ departamento | lowercase}}

# 6.3 Pipe decimal 

        El resultado es {{ resultado | number:’2.2-2’}}

# 6.4 Pipe Currency / Para definir tipo de  moneda
        {{ dolareuro | currency:'EUR':true}}

# ############################################
# 7 Servicios e Injección de dependencias / PROVIDERS
# ############################################
# ############################################
# 8 Routes
# ############################################
# ############################################
# 9 Forms
# ############################################
# 9.5 Validacón de campos programática 
 Es decir es una validación independiete de la validación de los atributos HTML5
 
    import validators en el componente que se desea usar

# ############################################
# 10 Server conection 
# ############################################
   Angular utiliza los métodos http para conectarse con el servidor

# 10.2 Servicio HTTP: Post     
  Se implementan por medio de un servicio
  
