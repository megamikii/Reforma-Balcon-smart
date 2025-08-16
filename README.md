# Reforma-Balcon-smart
Este es el incio de un git-vlog reformando, bueno mas bien terminando de decorar mi casa y haciendola inteligente usando home assistant.

## Primeros pasos (a lo capitan america)
Todo empezo queriendo construir dos paredes de pladur en el balcon para tapar la cristalera que nos separan del vecino, compramos dos placas de fibrocemento, los perfiles metalicos e incluso
los tornillos. Las placas las cortamos en el propio bauhaus, pero nos quedamos sin dinero y no podiamos comprar la pintura asi que dejamos las placas en en la terraza esperando que por gracia divina ahorrasemos y pudieramos comprar la pintura, cosa que no paso, las placas se pdudrieron en la terraza, y la masilla, que tambien compramos, tuvo mismo destino.
Despues de un tiempo decidi ponerme a  cortar aunque fuese los  perfiles, tengo la estructura del pladur practicmente hecha, sin atornillar.
Queriamos poner unas luces de navidad en la terraza pero no teniamos e.... ya lo pndre...

### Tareas hasta decidir decoracion final o cuando estemos solos.

#### Limpieza.

llevar al punto limpio, las bicis, la malla, alomejor colocar los azulejos en el zocalo de la cocina, colocar/limpiar las macetas.

#### Materiales.

Mirar si tengo materiales suficientes para lo que se pueda hacer antes de decidir la decoracion y empezar con el pladur. cables, tubos corrugaos, enchufes, cajas estancas...

#### Preinstalación electrica.

Marcar puntos de enchufes y cajas de conexiones, instalar tubos corrugados, dejar cajas de conexion superpuestas, todo el tema del wifi. Cambiar conexionado interruptor simple a triple. Llevar el encufe que esta ahora hasta la caja de conexion del sofa y colocarlo bien, en una clema, ya que ese sera el punto de donde salen todos los elementos electricos de la terraza. Alomejor meterlo en una caja estanca. Dejar preinstalado el caleado para tiras led cuando decida que voy a usar, para que cuando compre os materiales conectarlo y listo.

#### Pared.

Limpiar pared con estropajo, agua y jabon y aplicar el fijador sika08. El fijador se puede aplicar aunque no vallamos a pintar, creara una capa ya lista, cuando se pinte se limpia bien y listo.

#### Estructuras.

Ir montando la estructura de pladur que ya esta, y ponerle el liston de madera de refuerzo para la malla. pero en realidad no podemos porque hasta que compremos la placa de pladur va  a pasar mucho tiempo.

#### Domotica.

Poner el interruptor triple zigbee y las tiras led inteligentes (si las tengo ya comprada, para probarlas, aunque sea superpuestas) y el sensor de movimeto de la entrada, meterlas en home assistant y hacer automatizaciones y escenas.


### preinstalacion del conexionado electrico de la terraza:

Ahora mismo estoy focus en la parte electrica de la terraza, estos son los elementos que nos gustaria cambiar/poner: (todo es mientras mi novia y yo nos ponemos de acuerdo con la decoracion y la estructuracion de todo).

#### OBJETIVO:
Me gustaria poner un interruptor triple para separar ambientes, dos enchufes en el  sofa, y alomejor, una o dos tiras led en el techo y/o debajo del sofa. 

##### Para ello:
QUE NECESITO?
- Antes de nada limpiar: llevar al punto limpio, las bicis, la malla, alomejor colocar los azulejos en el zocalo de la cocina, colocar/limpiar las macetas, 
- Primero.Materales que necesito: cale de fase para el interruptor triple, cables neutro tierra y fase (2.5 de seccion) para los enchufes del sofa y las tiras led, tubo corrugado para protegerlos, caja de conexiones y alomejor alguna otra caja estanca para las conexiones, por lo tanto tengo que comprobar si tengo suficiente, medir el cable que necesito desde el interruptor triple a su caja de conexiones, cuanto necesito para llegar a la caj de conexiones de la terraza y de ahi a los enchufes y las tiras led y lo mismo para el tubo corrugado. Y fijaciones para el tubo corrugado.
- DOMOTICA: buscar tiras led inteligentes e interruptor triple zigbee y sensor de movimiento, porque asi no saturamos la wifi y empiezo a meterme en zigbee, aaa y meter home assistant en la raspberry y detactar el enchufe tapo que ya tengo en el salon.

- Segundo: tengo que cambiar las conexiones electricas del interruptor actual, al que le llega fase del cuadro electrico de la casa y sale un unico cable de fase hacia los tres puntos de luz, tengo que meterle dos cables mas de fase de salida, para dividirlos entre los tres faroles. Y neutro dependiendo de si el nuevo interruptor lo nocesita o no. Y si ya tengo el interruptor colocarlo, probarlo y meterlo en home assistant.

- Tercero: el enchufe que pusimos en su dia para las luces de navidad, en realidad son cables que vienen directamente del cudro electrico, los cuales hay que llevar por dentro del pladur hasta la caja de conexiones que estara dentro del sofa, tengo que dejar marcado en el suelo o en la cristalera por donde iran esos cables, la caja de conexiones, los puntos de luz para as tiras led, hay que decidir que vamos a poner y donde van a estar, y los enchufes del sofa.

- Cuarto: para este paso necesito ver si puedo meter cables ya o puede que se dañe al colocar el pladur, asi que llevar el tubo corrugado sin cable metido, a todos los puntos puestos en el paso anterior, dejar tubo corrugado hasta la caja de conexiones, de ahi a los dos enchufes del sofa y al punto de luz de las led, despues ver hasta donde llega el cable que ya esta para el enchufe, para intentar que llegue hasta la marca de la caja del paso anterior dejando como 50cm de cable extra. Protegiendo los extremos con cinta aislanteo incluso desconectando estos cables de la caja de conexiones naterior. Si veo que puedo dejar cable metido para el resto elementos, lo hago.

- Quinto: dejar el tubo fijado provisionalmente, al techo, y a la cristalera, dejar tambien superpuesta la caja de conexiones y dejar los tubos marcados, especificar para que es cada uno.

#### Conexionado tiras led.

##### Que leds voy a usar?.

De momento he encontrado estas dos opciones:
1. tira led govee/tapo... con su propio controlador/transformador, para el techo hay dos opciones: la facil es poner un enchufe escondidio en el falso techo y conectar la tira directamente y si quiero poner un interruptor seria ponerlo despues del enchufe, de esta manera el interruptor controlaria el enchufe, lo malo es que si apagas del interruptor la tria se queda sin electricidad por lo tanto podria desconectarse home assistant y que al volverla a encender no la detecte de nuevo.

2. tira led aliexpres + controlador esp32 con wled (aliexpress) + fuente de alimentacion 12/24v 60-100w (aliexpress), mas complicado por ser un proyecto diy,pero lo conctaria directamente a toma electrica que venga del interruptor,lo puedo poner como me de la gana, tamaño de la tira, colores esxcneas automatizaciones... lo malo es que si apagas del interruptor la tria se queda sin electricidad por lo tanto podria desconectarse home assistant y que al volverla a encender no la detecte de nuevo. Creo proque tengo que investigar mas


##### Conexionado electrico.

Las tiras led inteligentes llevan, la propia tira led, un cotrolador, que es el que se encarga de comunicarse con home assistant, un transformador de 12v a 230v y el enchufe.
La mayor parte de las tiras led llevan el transformador y el enchufe juntos, mo puedo cortar los cable del enchufe oelarlos y conectarlos a la salida del interruptor que las encienda, entonces:

##### Como lo puedo hacer??.

Tengo que decidir entre:
   - Controlar la tira led desde el móvil. Entonces la primera opcion seria;
   conectar la tira led directamente a los cables wue vienen de la caja de conexiones.
   problemas: las tiras led tiene transformador y enchuefe en una misma pieza, tedria que cortarlos y comprar un transformador 12/24v conectarlo a la tira led y de el a los cables de 230v directamente, prediendo la garantia de la led.
   La segunda opcion seria:
   poner un enchufe dentro del sofa para la led del sofa, o dentro del falso techo para la led de la terraza, conertar la tira led a ellos sin cortar nada.
   problemas: es mmas chapuza, porque guay es conertarlas directamente a la red, aunque si que es cierto que las tiras led inteligentes, normalemente se enchufan en vez conectarlas a la red directamente. El otro problema es que el enchufe del falso techo estari mas expuesto a la lluvia, creo, porque al final esta dentro del falso techo, no se yo...
   - Contraolarla desde un interruptor y el móvil.
       conectar la tira led directamente a los cables wue vienen de la caja de conexiones, poniendo un interruptor en medio. Entonces la primera opcion seria:
    problemas: las tiras led tiene transformador y enchuefe en una misma pieza, tedria que cortarlos y comprar un transformador 12/24v conectarlo a la tira led y de el a los cables de 230v directamente, prediendo la garantia de la led.
  La segunda opcion seria:
   poner un enchufe dentro del sofa para la led del sofa, o dentro del falso techo para la led de la terraza, conectar la tira led a ellos sin cortar nada y en entre ellos un interruptor.
   problemas: es mmas chapuza, porque guay es conertarlas directamente a la red, aunque si que es cierto que las tiras led inteligentes, normalemente se enchufan en vez conectarlas a la red directamente. El otro problema es que el enchufe del falso techo estari mas expuesto a la lluvia, creo, porque al final esta dentro del falso techo, no se yo.
  La tercera opción seria, usar el controlador, que normalmente lleva botones, como interruptor. Para ponerlo en el sofa seria buena idea, porque puedo conectarala a red directamente, ya que la caja de conexiones estara ahi, usando sus propios botones como interruptor y poniendolo debajo del sofa. Pero para el techo, nose puede, porque habri que alargar el cable que va de la tira al controlador, pero esos cables son especaile y no se pueden extender mas de dos metros, asi que solo me vale para la tira del sofa.
#### Domótica.
buscar tiras led inteligentes e interruptor triple zigbee, porque asi no saturamos la wifi y empiezo a meterme en zigbee, aaa y meter home assistant en la raspberry y detactar el enchufe tapo que ya tengo en el salon.

### PROYECTOS.
#### pladur.
#### Malla y ventanas.
#### Tendedero.
#### Pared.
#### Sofá.
#### Mesa extensible/plegable?.
#### Domótica.
#### Techo.
#### Toldo/stores DIY/estoresIKEA...
#### Armario de herramientas.
#### GymCat.
#### Decoración.
