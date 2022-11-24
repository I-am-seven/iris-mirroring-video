# iris-mirroring-video
Video tutorial IRIS


Se debe crear una carpeta llamada "Licencias" donde se debe dejar el archivo .key

## Comandos
Primario: docker run -dt -p 8773:52773 -p 8972:1972 --name primario -h primario irisdemo:1.1 --check-caps false

Secundario: docker run -dt -p 9773:52773 -p 9972:1972 --name secundario -h secundario irisdemo:1.1 --check-caps false

Arbitro: docker run -dt --name arbitro -h arbitro localhost/intersystems/arbiter-arm64:2022.1.1.374.0 --check-caps false


##Nota:
  - La versión de la imagen oficial de IRIS es intersystems/iris-arm64:2022.1.0.209.0
  - La versión de la imagen del arbitro es localhost/intersystems/arbiter-arm64:2022.1.1.374.0
  - Ambas versiones estan en el registry de InterSystems
  - Yo use la versión para ARM de IRIS, ya que hice este tutorial en una Mac con procesaro M1
