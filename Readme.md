# Descripción de los archivos

Este repositorio contiene una serie de archivos que proporcionan funcionalidades comunes para aplicaciones desarrolladas con React. A continuación, se explica el propósito y funcionamiento de cada uno de estos archivos.

## 1. `useCounter.js`

Este archivo proporciona un hook personalizado llamado `useCounter`, que permite manejar un contador dentro de un componente de React. Este hook devuelve un objeto con el estado del contador y funciones para aumentar, disminuir y restablecer su valor.

### Funciones proporcionadas por `useCounter`:

- `counter`: Almacena el valor actual del contador.
- `Aumentar(valor)`: Incrementa el contador por el valor especificado o por 1 si no se proporciona ningún valor.
- `Decrementar(valor)`: Decrementa el contador por el valor especificado o por 1 si no se proporciona ningún valor. No permite que el contador caiga por debajo de cero.
- `Reset()`: Restablece el contador a su valor inicial.

## 2. `useFetch.js`

Este archivo proporciona un hook personalizado llamado `useFetch`, que facilita las solicitudes HTTP y maneja la lógica de carga de datos de una API externa en un componente de React. Devuelve un objeto con el estado de la solicitud, incluyendo los datos recuperados, el estado de carga y cualquier error que pueda ocurrir.

### Funciones proporcionadas por `useFetch`:

- `data`: Almacena los datos recuperados de la solicitud.
- `isLoading`: Indica si la solicitud está en curso.
- `hasError`: Almacena cualquier error que ocurra durante la solicitud.

## 3. `useForm.js`

Este archivo proporciona un hook personalizado llamado `useForm`, que simplifica la gestión de formularios en componentes de React. Devuelve un objeto con el estado del formulario y funciones para actualizar los valores de los campos y restablecer el formulario.

### Funciones proporcionadas por `useForm`:

- `fromState`: Almacena el estado actual del formulario.
- `onInputChange(evento)`: Actualiza el estado del formulario cuando se produce un cambio en un campo de entrada.
- `onReset()`: Restablece el estado del formulario a sus valores iniciales.

## 4. `useTodo.js`

Este archivo proporciona un hook personalizado llamado `useTodo`, que facilita la gestión del estado de una lista de tareas (todos) en una aplicación de React. Utiliza un reducer para manejar las acciones sobre la lista de tareas y también utiliza el almacenamiento local para persistir los datos.

### Funciones proporcionadas por `useTodo`:

- `handleNewTodo(todo)`: Agrega una nueva tarea a la lista.
- `handleDeleteTodo(id)`: Elimina una tarea de la lista según su ID.
- `handleToggleTodo(id)`: Cambia el estado de completitud de una tarea en la lista.
- `pendingTodosCount`: Devuelve la cantidad de tareas pendientes en la lista.
- `todos`: Almacena la lista de tareas actual.
- `todosCount`: Devuelve la cantidad total de tareas en la lista.

## 5. `todoReducer.js`

Este archivo define el reducer utilizado por `useTodo.js` para gestionar las acciones sobre la lista de tareas. El reducer define cómo cambia el estado de la lista de tareas en función de las acciones recibidas.

Espero que esta descripción ayude a entender el propósito y funcionamiento de cada archivo en este repositorio.
