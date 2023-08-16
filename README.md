# Carteis LED 
Repositorio cos deseños dos carteis feitos con tiras LED
Neste repo subiremos a información para fabricar os carteis que deseñamos no IES de Teis desde decembro de 2022.

Cartel do IES de Teis 
O primeiro modelo foi construido para inaugurar as vacacións de nadal Abel's stile.
![cartelIESTeis1](https://github.com/tecnoteis/carteisLED/assets/126872606/90f26060-75cd-4b8d-a0f1-b900b50c9e4c)
Consiste nunha serie de letras impresas en 3D con tapas de metacrilato cortadas coa cortadora láser e ancladas a unha base de DM tamén cortada coa láser. Cada letra ten, no interior, tiras LED WS2812B unidas en serie mediante cableado que vai dentro da base. A controladora é unha Arduino UNO R3, pero pode ser calquera que manexe a bilioteca de Adafruit para os Neopixel, que utilizamos para controlar os xogos de cores que fai o cartel.
As letras foron deseñadas en Onshape: https://cad.onshape.com/documents/4773bc60c2ff5bee8ad740b4/w/625422397d679016f6e905c3/e/1a73bd1ce32b01c9ed044d96?renderMode=0&uiState=64dc978b4a5b7726a82d2d40
Necesitas unha conta de Onshape para copiar nela os deseños e na documentación hai un vídeo titorial con instrucións para crear as letras que necesites.
A tira de LEDs conéctase segundo o esquema que podes ver no cartafol "Documentación". Ten un sentido de conexión, podes cortar tantos tramos como necesites, pero hai un lado que é a entrada e outro a saida da alimentación e a programación, por dicilo dalgunha maneira.

![cableadoLetraE](https://github.com/tecnoteis/carteisLED/assets/126872606/d5cce52f-a4be-45d2-9d9b-ae39d889e4ff)


Cada letra ten un burato para a entrada dos cables e outro para a saída, e as tiras LED están colocadas tendo en conta a entrada e saída.
A tapa das letras tamén está en Onshape, e poden ser cortadas en metacrilato traslúcido coa cortadora láser ou poden ser impresas en 3D en plástico branco ou traslúcido. Neste caso recomendamos cambiar o deseño das letras para que o encaixe sexa de 1 mm e non de 3 mm , que é o grosor do metacrilato. Con tapas de PLA de 1 mm ou menos, a luz dos LEDs queda ben.
No cartafol "Titoriais" tedes o titorial para modificar os deseños das letras.
Para a base utilizamos un deseño de caixas, con encaixes tipo dedo, obtido da web makercase.com. Utilizamos DM de 3mm e o tamaño necesario para soportar as letras.

![baseCartel](https://github.com/tecnoteis/carteisLED/assets/126872606/b7c1ad6e-1371-47f6-84dd-89f3e27168e1)


Carteis con mensaxe

Como colaboración co grupo de Igualdade do IES de Teis elaboramos dous modelos de carteis, unha caixa de DM para o espazo de reunión do grupo e outro modelo con electrónica móbil, que servira para múltiples mensaxes.
![carteisAcesos](https://github.com/tecnoteis/carteisLED/assets/126872606/829bf531-d928-40c7-8de9-f0dda3e5335d) ![inteirosAcesp](https://github.com/tecnoteis/carteisLED/assets/126872606/e53344ad-6c52-4df5-b939-6e4d4b0454b5)

A caixa de DM creámola na web makercase.com e cortámola coa láser e as caixas de cartón son caixas de portátiles edixgal pintadas e cortadas coa láser.
A electrónica ten o mesmo esquema que o cartel do IES de Teis, pero está pegada a unha base rectángular, tal como podes ver na imaxe.
![panelLED](https://github.com/tecnoteis/carteisLED/assets/126872606/532e0bc1-bf5f-4c8e-8691-84145f515a18)

A alimentación pode ser con baterías recargables 18650 ou cunha fonte de alimentación conectada á placa Arduino.
Nun dos carteis utilizamos un powerbank conectado como nos mClons: https://tecnoloxia.org/mclon/alimentacion/powerbank/

O programa que fai que a tira de LED faga distintos xogos de cores e intensidades é unha modificación do exemplo "RGBWstrandtest" incluido na biblioteca de Adafruit para as tiras de LED Neopixel. Podes descargar aquí a biblioteca para instalala no IDE de Arduino e o programa de exemplo, aínda que xa aparece despois de instalar a biblioteca. No programa só tes que modificar o pin no que está conectado o pin data da tira de LED e o número total de LED da tira. Despois podes xogar co brillo ou co que queiras.

