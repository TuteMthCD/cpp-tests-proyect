# Proyecto Template C++

Este repositorio funciona como un _template_ mínimo para proyectos en C++ que usan **CMake** y **GoogleTest**.

## Copiar o clonar

Puedes obtener una copia ejecutando:

```bash
git clone <url-del-repositorio> mi-proyecto
```

Luego entra en la carpeta creada para comenzar a trabajar.

## Compilar y ejecutar

Desde la raíz del proyecto ejecuta los siguientes comandos:

```bash
cmake . -B build
cd build
make
make run
make test
```

- `make` compila la aplicación y las pruebas.
- `make run` ejecuta el binario principal.
- `make test` corre las pruebas unitarias.

