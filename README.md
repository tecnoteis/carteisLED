# carteisLED
Repositorio cos deseños dos carteis feitos con tiras LED
Neste repo subiremos a información para fabricar os carteis que deseñamos no IES de Teis desde decembro de 2022.

O primeiro modelo foi construido para inaugurar as vacacións de nadal Abel's stile.
![cartelIESTeis1](https://github.com/tecnoteis/carteisLED/assets/126872606/90f26060-75cd-4b8d-a0f1-b900b50c9e4c)
Consiste nunha serie de letras impresas en 3D con tapas de metacrilato cortadas coa cortadora láser e ancladas a unha base de DM tamén cortada coa láser. Cada letra ten, no interior, tiras LED WS2812B unidas en serie mediante cableado que vai dentro da base. A controladora é unha Arduino UNO R3, pero pode ser calquera que manexe a bilioteca de Adafruit para os Neopixel, que utilizamos para controlar os xogos de cores que fai o cartel.
As letras foron deseñadas en Onshape: https://cad.onshape.com/documents/4773bc60c2ff5bee8ad740b4/w/625422397d679016f6e905c3/e/1a73bd1ce32b01c9ed044d96?renderMode=0&uiState=64dc978b4a5b7726a82d2d40
Necesitas unha conta de Onshape para copiar nela os deseños e na documentación hai un vídeo titorial con instrucións para crear as letras que necesites.
A tira de LEDs conéctase segundo o esquema que podes ver no cartafol "Documentación". Ten un sentido de conexión, podes cortar tantos tramos como necesites, pero hai un lado que é a entrada e outro a saida da alimentación e a programación, por dicilo dalgunha maneira.

![cableadoLetraE](https://github.com/tecnoteis/carteisLED/assets/126872606/d5cce52f-a4be-45d2-9d9b-ae39d889e4ff)


Cada letra ten un burato para a entrada dos cables e outro para a saída, e as tiras LED están colocadas tendo en conta a entrada e saída.
