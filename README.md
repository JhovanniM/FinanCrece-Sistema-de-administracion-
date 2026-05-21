# FinanCrece-Sistema-de-administracion-
Sistema Profesional de Gestión de Préstamos Personales
> Este codigo está diseñado para que un prestamista pueda llevar el control exacto de su dinero, sus clientes, las fechas de cobro y sus ganancias

1. main.py (Es el Motor de Arranque)
Es el archivo a ejecutar. El trabajo del main es asegurarse de que la computadora tenga las herramientas necesarias para mostrar la interfaz (ttkbootstrap) y las gráficas (matplotlib). Si detecta que falta algo, lo instala. Luego, inicializa la aplicación.

2. backend.py (El Cerebro y la memoria)
   
Aquí es donde ocurre toda la magia. Hace dos cosas principalmente:

Base de datos: Crea y gestiona un archivo llamado prestamos.db de forma automática. Ahí guarda de forma permanente a los clientes, cuánto dinero se tiene prestado, los pagos que han hecho y cuánto capital queda.

Matemáticas y Lógica: Cuando se aprueba un préstamo, este archivo calcula instantáneamente de cuánto será cada cuota, cuánto ganará de interés y en qué fecha terminará de pagar el cliente. También se encarga de restar el dinero del "capital físico" y alerta si se está prestando dinero que no se tiene (Deuda del dueño).

3. frontend.py (La Cara Visible / Interfaz Gráfica)
Es todo lo visible y todo lo que se toca en la pantalla. Utiliza una librería que le da ese aspecto moderno.

Login: La pantalla inicial de seguridad donde pone el logo de la empresa prestamista y el usuario y la  contraseña.

Módulos (Botones Laterales): Crea las ventanas donde se  registra clientes, ver quién debe pagar el día de hoy, y marcar pagos con un solo clic (✅ Pagó, ⚠️ Parcial, ❌ No Pagó).

Gráficas: Toma los datos matemáticos del backend y dibuja gráficas visuales (pasteles y barras) para ver  rápidamente en qué zonas se  tiene más dinero prestado y si el negocio está creciendo.
