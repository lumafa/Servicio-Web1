# Mi Nuevo Proyecto Git
Contenido de prueba para mi nuevo repositorio.
Diseño y desarrollo de sericios web para un registro y un inicio de sesión, el servicio recibe un usuario y contraseña, la autenticación correcta dice satisfactoria y si es incorrecta me dice error en la autenticación. El codigo contiene comentarios y utilizo herramientas de versionamiento.
Estructura del proyecto
server.js: Punto de entrada. Inicializa el servidor Express, establece la conexión con MongoDB y define las rutas principales.
models/User.js: Modelo de Datos. Define la estructura de los usuarios (nombre, apellidos, correo, password y celular) y asegura que el correo sea único.
controllers/auth.controller.js:	Lógica de Negocio. Contiene las funciones de register (para crear y encriptar la contraseña) y login (para autenticar al usuario comparando la contraseña encriptada).
routes/auth.routes.js:	Define los endpoints /api/register y /api/login.

Registro (/api/register) Resultado-	Éxito: El usuario fue creado y guardado en la base de datos.	Respuesta de Postman: "Usuario registrado exitosamente."

nicio de Sesión (/api/login)	Resultado -- Éxito: Se validó la contraseña correctamente (gracias a bcryptjs).	Respuesta de Postman: "Autenticación satisfactoria. ¡Bienvenido!"
