# ep1dp24_Leslie_Sanchez
Creación de clases
class Continente:
    def __init__(self, codigo_continente, nombre_continente):
        self.codigo_continente = codigo_continente
        self.nombre_continente = nombre_continente


class Pais(Continente):
    def __init__(self, codigo_continente, nombre_continente, codigo_pais, nombre_pais):
    super().__init__(codigo_continente, nombre_continente):
    self.codigo_pais = codigo_pais
    self.nombre_pais = nombre_pais


class Empresa(Pais):
    def __init__(self, codigo_continente, nombre_continente, codigo_pais, nombre_pais, codigo_empresa, nombre_empresa, telefono_empresa):
        super().__init__(codigo_continente, nombre_continente, codigo_pais, nombre-pais):
        self.codigo_empresa = codigo_empresa
        self.nombre_empresa = nombre_empresa
        self.telefono_empresa = telefono_empresa


class Representante(Empresa):
    def __init__(self, codigo_continente, nombre_continente, codigo_pais, nombre_pais, codigo_empresa, nombre_empresa, telefono_empresa, codigo_representante, nombre_representante):
    super(). __init__(codigo_continente, nombre_continente, codigo_pais, nombre_pais, codigo_empresa, nombre_empresa, telefono_empresa):
    self.codigo_representante = codigo_representante
    self.nombre_representante = nombre_representante

Creación de objeto
def crearRegistro():
    codigo = input("Ingrese el código: ")
    nombre = input("Ingrese el nombre: ")
    telefono = input("Ingrese el teléfono: ")
    codigo_representante = input("Ingrese el código del representante: ")
    nombre_representante = input("Ingrese el nombre del representante: ")
    return Representante(codigo, nombre, telefono, codigo_representante, nombre_representante)


if __name__ == "__main__":
    registros = []
    for _ in range(2):
        registro =crearRegistro()
        registros.append(registro)


    for registro in registros:
        print(f"Representante: {registro.nombre_representante}")
