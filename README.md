# Puntuacion por tiempo vivo
class SistemaPuntuacion:
    def __init__(self):
        self.puntuacion = 0

    def agregar_puntos(self, puntos):
        self.puntuacion += puntos

    def restablecer_puntuacion(self):
        self.puntuacion = 0

    def obtener_puntuacion(self):
        return self.puntuacion

# Crear una instancia del sistema de puntuación
sistema_puntuacion = SistemaPuntuacion()

# Función para simular perder el juego y reiniciar la puntuación
def perder_juego():
    print("Has perdido el juego.")
    sistema_puntuacion.restablecer_puntuacion()

# Ejemplo de uso
sistema_puntuacion.agregar_puntos(10)
print(f"Puntuación actual: {sistema_puntuacion.obtener_puntuacion()}")

# Simular perder el juego
perder_juego()

# La puntuación se ha reiniciado
print(f"Puntuación después de perder: {sistema_puntuacion.obtener_puntuacion()}")
