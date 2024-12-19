# Proyecto Examen DSA - Backend y Android David Lamas Pregunta (2)

Este proyecto fue realizado como parte del examen para la asignatura de **Diseño de Sistemas de Aplicaciones (DSA)**, donde se implementa tanto un backend en Java como una aplicación Android que consume una API REST.

## Backend

En el backend, se ha desarrollado una API que devuelve un JSON con un `GET` en la clase `UserService`. Este `GET` proporciona tres oraciones de ejemplo. Para comprobar su correcto funcionamiento, se ha utilizado **Swagger**, confirmando que el endpoint devuelve la información correctamente.

### Estructura Backend

- **UserService**: Clase que gestiona el endpoint que devuelve las oraciones de ejemplo en formato JSON.
- **Swagger**: Se utilizó Swagger para verificar el correcto funcionamiento del endpoint GET.
  
## Android

En la parte de Android, se ha modificado la aplicación existente para agregar una nueva funcionalidad que, después de iniciar sesión, redirige al usuario a una nueva actividad donde se muestran los mensajes obtenidos desde el backend.

### Características

- **Nuevo botón en la pantalla de inicio de sesión**: Después de que el usuario inicie sesión correctamente, se agrega un botón que redirige a la actividad donde se mostrarán los mensajes.
- **Llamada a la API**: La nueva actividad realiza una llamada al endpoint GET del backend para obtener los mensajes.
- **Manejo de errores**: Si la llamada a la API no es correcta, se muestra un mensaje `Toast` con la información correspondiente.

### Componentes en Android

- **Clase Mensaje**: Representa el modelo de datos para los mensajes que se muestran en la actividad.
- **APIService**: Interfaz que contiene la URL del endpoint GET de la API para obtener los mensajes.
- **MessageAdapter**: Adaptador que maneja la visualización de los mensajes en la interfaz de usuario.
- **Actividad de mensajes**: Actividad que maneja la visualización de los mensajes y la interacción con el backend.

## direcciones IP

- **Backend**: localhost:8080
- **Android**: 10.0.2.2:8080

## direcciones IP
- No se muy bien que versión de java y android estoy utilizando, cabe tenerlo en cuenta para ciertas sintaxis sobre todo de JAVA.

