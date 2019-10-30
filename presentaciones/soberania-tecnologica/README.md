# Blockchain

# Blockchain

Es un sistema de almacenamiento de información seguro y descentralizado.

Esta información está representada en forma de transacciones, y éstas son agrupadas en estructuras de datos llamadas bloques.

Toda la magia radica en el modo en que la información es añadida y almacenada en el blockchain, que produce algunas características altamente deseables:

- Inmutabilidad de la historia.
- Invulnerabilidad del sistema.
- Persistencia de la información.
- No hay un solo punto de falla.

## Estructura de almacenamiento

Como su nombre lo indica, block (bloques) chain (cadena), es una cadena de bloques enlazados mediante algoritmos criptográficos que aseguran su inmutabilidad.

Esto significa que cada bloque guarda su propio HASH como némero de identificación, y el del bloque anterior, de manera que están enlazados hasta el primer bloque de la blockchain.

## Funcionamiento y actualización de los datos

### Cómo se agrega un nuevo bloque a la red?

Blockchain se mantiente mediante una red distribuída de nodos que generan y validan transacciones.

1- Se genera una transacción entre usuarios de la red
Se firma digitalmente.

2- Luego de que se crea es propagada y validada por la red (la mayoría de los nodos) para finalmente ser agregadas a un bloque.

3- Cuando un bloque está listo para ser agregado a la red,
entran en juego los mecanismos de consenso establecidos, de manera que los nodos encargados de validar la actualización de la red, recurren a ellos para validar o desechar bloques.

Existen distintos **mecanismos de consenso**, uno de ellos es el **Proof-of-Work** (prueba de trabajo), que consiste en una serie de **operaciones criptográficas** sobre un bloque.

Estas operaciones tienen un **alto coste computacional**, lo que garantiza que el nodo ha invertido fuerza de cómputo y tiempo (en otras palabras, energía y dinero) en validar el bloque.

4- Los bloques que han sido validados por varios nodos de la red (consenso) acaban integrándose en la cadena de bloques que funciona como una una base de datos completamente descentralizada que ningún nodo de la red podría manipular sin el consenso de la mayoría de los nodos.

Cada bloque nuevo también se transmite por toda la red, de modo que todas las copias de todos los nodos de la red tengan el mismo conjunto de datos de todas las transacciones, garantizando la **integridad de la informacion**.

La forma en que estos bloques son encadenados es a través del uso de un método conocido como **hashing**. Consiste fundamentalmente en una función que toma como parámetro un bloque y luego de aplicar algunos algoritmos matemáticos produce una salida llamada hash.

El hash resultante de cada bloque es agregado como parte de la información del siguiente bloque. De esta forma se evita que los bloques en el medio de la cadena sean falsificados. Cualquier cambio en su contenido cambiaría el valor del hash calculado y por lo tanto no coincidiría con el valor existente en el siguiente elemento.

![](https://i.imgur.com/mCmJJX3.png)

## Características

#### Descentralización

Una red blockchain está estructurada en base a <b>nodos descentralizados</b> con <b>capacidad de procesamiento</b> y almacenamiento

Cada nodo guarda una **replica** de todo el **historial de transacciones**

Esto permite que no haya una autoridad única regulatoria de los datos en tanto la cadena de bloques se mantiene actualizada debido a la propagación que se realiza cada vez que hay nuevos registros.

Todos los miembros de la red pueden proponer nuevos bloques a ser agregados, siendo el trabajo del resto de los nodos aceptarlo o no como válido. La mayoría decidirá si la cadena es finalmente actualizada. Este proceso se conoce como **consenso**.

#### Inmutabilidad de los datos

La clave de su funcionamiento tiene que ver con la combinación de la **criptografía de clave pública**, los **hashes criptográficos** y los mecanismos de consenso adoptados.

Por un lado, hace uso de una **pareja de claves** (**pública y privada**) para **cifrar** nuestras transacciones.

El wallet o monedero de una criptomoneda, por ejemplo, no es otra cosa que una pareja de claves. La clave pública es la dirección donde se pueden recibir transferencias de valor. La clave privada, en cambio, se utiliza para firmar operaciones de salida, de un modo similar a cuando firmamos un documento con un certificado o un correo electrónico con PGP.

Con la criptografía de clave pública se garantiza la **integridad y autenticidad de la información** que se almacena en cada transacción.

La información cifrada de las transacciones se agrupa en los **bloques** (blocks) que se van **encadenando** (chain) a medida que los nodos van **verificando** las transacciones.

## Bitcoin, la primer blockchain

En 2009, un artículo titulado _Bitcoin: un sistema de dinero electrónico peer-to-peer_ fue publicado por un individuo (o tal vez un grupo) llamado Satoshi Nakamoto. El artículo combinaba **técnicas criptográficas** y una **red peer-to-peer** sin la necesidad de confiar en una autoridad centralizada (como los bancos) para realizar pagos de una persona a otra.

En Bitcoin las transacciones están basadas en el traspaso de valor entre billeteras o wallets de usuarios participantes.
Por lo tanto la información que es persistida en la Blockchain de Bitcoin está compuesta fundamentalmente por direcciones de origen/destino y montos transferidos.

La plataforma Bitcoin fue la primera en aplicar y popularizar la tecnología de bloques, que, sin embargo, tiene un campo de aplicación mucho más amplio que únicamente pagos o criptomonedas.

---

## Desarrollo basado en Blockchain

### Blockchain frente a las bases de datos tradicionales

Blockchain puede entenderse como una capa de datos para sus aplicaciones. Esta puede ser la única capa de persistencia, sin embargo también puede ser una de múltiples de diferentes tipos.

Las bases de datos tradicionales tienen modelos para modelar los datos como tablas, o inclusive documentos. Las blockchains en general no deben adherirse a esta convención ya que parecen más una base de datos noSQL donde los datos se pueden guardar con cualquier formato que desee, lo que no quita que se establezcan algunos estandares o modelos.

Otra buena comparación en la línea de bases de datos y probablemente la más importante son los procedimientos almacenados. Los procedimientos almacenados son lógica (funciones) viviendo en la misma base de datos, recibiendo entradas para ejecutar operaciones con los datos. En el lenguaje blockchain a esto se le llaman contratos inteligentes (smart contracts) o chaincode.

Blockchain es descentralizado y la ejecución de un contrato inteligente debe suceder en múltiples ocasiones en diferentes computadores, esos son parte de los conceptos de computación distribuida que un desarrollador debe tomar en cuenta cuando utiliza blockchain como una capa de datos.

### Ethereum

Como **Bitcoin**, **Ethereum** es una red distribuida de cadena de bloques pública.
Innova al expandir las posibilidades de las aplicaciones de la tecnología Blockchain

- Permite crear e implementar **DApps** - Tiene una criptomoneda propia: el Ether - La plataforma se enfoca en ejecutar el código de programación de cualquier aplicación descentralizada. - Hay un Ethereum Virtual Machine (EVM) corriendo en cada nodo de Ethereum compilando DApps.

Antes de la creación de Ethereum, las aplicaciones de cadena de bloques fueron diseñadas para hacer un conjunto limitado de operaciones. Bitcoin y otras criptomonedas, por ejemplo, fueron desarrolladas exclusivamente para operar como monedas digitales entre pares.

La red de Ethereum está compuesta por dos tipos de nodos denominados **full nodes** y **light nodes**.

Los full nodes contienen la **historia completa de transacciones** desde el bloque Génesis. Son la prueba de integridad de la red Blockchain y por lo tanto se encargan de verificar todas las transacciones y los bloques.

Por otro lado, los light nodes solo contienen un subconjunto de transacciones y son utilizados como wallets. Estos nodos no verifican las transacciones y se ayudan de los full-nodes para obtener datos que puedan necesitar.

Dentro de cada uno de estos nodos se ejecuta un software llamado Ethereum Virtual Machine (EVM). Esta máquina virtual se encarga de mantener los datos de la Blockchain sincronizados y además provee el ambiente para la ejecución del código de las aplicaciones de los usuarios.

Ethereum es una plataforma abierta de software basada en la tecnología de cadena de bloques que permite a los desarrolladores crear e implementar aplicaciones descentralizadas. Esta plataforma se enfoca en ejecutar el código de programación de cualquier aplicación descentralizada.

Dado que los contratos inteligentes desempeñan una función lógica (if-this.than-that), necesitan de una situación y de su desarrollo para conseguir cumplir estas condicciones. Las dApps tienen la necesidad de obtener informaciones precisas desde el mundo que le rodea, y Ethereum es ese servicio que las conecta con datos reales.

Ethereum es también usado como plataforma para crear otras criptomonedas.

### Dapps

_DApp_, acrónimo de **aplicación descentralizada**: su código backend es ejecutado en una red descentralizada peer to peer basada en blockchain, como podría ser Ethereum.

Es decir, su funcionamiento no depende de puntos de control o servidores centrales, sino que funciona en base a una **red descentralizada**.

No dependen de un servidor ni autoridad central para su creación o ejecución.

En las DApps, el backend está relacionado a un smart contract que se ejecuta sobre una blockchain, por ejemplo Ethereum. De esta forma, un smart contract tiene una programación que garantiza el funcionamiento de la DApp.

La aceptación o no de las operaciones realizadas por los usuarios de la DApp, va supeditada a la programación de dicho smart contract.

En este caso, cada usuario de la DApp es un nodo dentro de la red.

Al ser los smart contract visibles y públicos, esto garantiza un alto nivel de transparencia y seguridad. Los usuarios pueden estar seguros que la DApp no hará nada distinto a lo que especifica el smart contract.

El backend es soportado por las API (Interfaz de Programación de Aplicaciones) y capacidades de la blockchain con la que se interactúa, como puede ser la red Ethereum, que provee distintos servicios para el desarrollo de dapps.

En cuanto al almacenamiento de los datos, también es completamente descentralizado. Cada usuario de la DApp almacena un historial completo de las acciones que se realizan en la red DApp, y a su vez, las interacciones son almacenadas en la blockchain dentro de los bloques de la misma. Para ello se utilizan técnicas criptográficas que garantizan accesos seguros.

##### Ejemplo:

Para pensar una diferencia respecto a las aplicaciones ceentralizadas, en los servicios que éstas proveen, los datos y decisiones se toman en unos servidores centrales. En todos esos servicios, los datos y decisiones se toman en unos servidores centrales. Esto le permite a la empresa detrás de esos servicios, tomar acciones de censura, alteración del comportamiento, o incluso beneficiar o perjudicar únicamente a determinados usuarios poniendo en constante tela de juicio la neutralidad e igualdad de condiciones.

### Smart Contracts

El código que se desarrolla, inicialmente en un lenguaje de alto nivel para luego ser ejecutado en la EVM, se denomina Contrato Inteligente o Smart Contract.

Estos contratos no solo son representados digitalmente sino que también es posible hacerlos actuar en base a determinados eventos, es por eso que son “inteligentes”. Tener estos contratos como parte de la Blockchain asegura que el contrato no puede ser modificado y que las condiciones acordadas serán ejecutadas inevitablemente.

---

## Demo

1. #### Instalamos ambiente de desarrollo de smart contracts con Ethereum
2. #### Desarrollamos una dapp simple con VueJs que necesite almacenar datos, usando Truffle para conectarnos a la blockchain.
3. #### Escribimos un smart contract que garantice la lógica de negocio de la dapp
4. #### Levantamos red privada blockchain con Ganache
5. #### Deployamos el contrato en la red que simula Ganache

###### Truffle y Ganache proveen:

- Compilación de smart contracts.
- Automatización del testeo de contratos.
- Automatización del deploy de smart contracts.
- Gestión de las redes de Ethereum para deployar los smart contracts, ya sean públicas o privadas.

---

## El Futuro

Acá hay 3 ámbitos en los que podríamos aplicar Blockchain y nos solucionarían ciertos problemas que nos vamos a encontrar de acá a 10 años.

- **Sanidad** : Hoy en día, toda nuestra información y estudios sanitarios quedan archivados en los servidores del hospital donde vayamos. La realidad es que nuestro expediente medico podria estar descentralizado en una red blockchain pudiendo acceder de manera agil y yo decidiria quien puede ver mi expediente medico.

- **Internet de las cosas**: El modelo centralizado no va a soportar miles de millones de dispositivos conectados a internet. Sumado a esto, yo quisiera que este dispositivo se conecte directamente conmigo. Esto lo soluciona blockchain.

- **Bienes digitales**: Por ejemplo, entradas de cine que saque via web. El problema, es que es muy dificil comprobar quien es el dueño realmente de esa entrada. Blockchain soluciona esto perfectamente.

## Blockchain para video juegos

Datos inmutables, registos históricos y dinero real.
Ofrecen una experiencia descentralizada de juego.

Algunas categorías:

- como una recompensa para el juego
- como una herramienta promocional artificiosa
- o como un verdadero modificador del juego

##### Ejemplos

###### Recompensa por jugar ciertos juegos en línea:

- Lanzamiento del equipo de la moneda de los servidores de Counter Strike y Minecraft

###### Diseño de juegos con criptomoneda o blockchain en mente como recompensa por jugar o como medio de pago:

- TurboCharged
- FlapPig
- SaruTobi

###### Juegos ofreciendo recompensas Bitcoin:

- Grabbit
- BitQuest

##### Sistema propio de recompensas:

- Spells of Genesis: utilizando su propia moneda BitCrystals y blockchain para guardar (y para garantizar la autenticidad de) las tarjetas coleccionables.

- CryptoKitties: mascotas digitales únicas. Incorporó su criptomoneda Kin, permitiendo que cualquier desarrollador de juegos use Kin como un token de recompensa.

---

### Tutoriales para introducirse en el desarrollo Blockchain

- Laboratorio [dapp](https://docs.google.com/document/d/1WfB6a6yXWmdtRu7RM96kR2TZi-cyLycjP2DMKt5SiDQ/edit) en Ethereum. [Repositorio](https://github.com/nefera606/BlockchainForDevelopers) en Github.
- [Ejemplo](https://medium.com/coinmonks/getting-started-with-solidity-development-using-truffle-2cc6c1df9133) de smart contract para Ethereum.
- [Ejemplo](https://www.returngis.net/2019/05/desarrollando-smart-contracts-para-ethereum-con-truffle/) de smart contract con Truffle.
- Create [blockchain dapp con Vuejs](https://www.danielefavi.com/create-your-blockchain-dapp-with-ethereum-and-vuejs-part-1/) para Ethereum. [Repositorio](https://https://github.com/danielefavi/ethereum-vuejs-dapp) en Github.
- [Desarrollo de una dapp de votacion](https://aprendeblockchain.wordpress.com/desarrollo-en-ethereum/desarrollo-con-truffle-i/) con Truffle.
- [Blockchain development](http://www.dappuniversity.com/articles/blockchain-developer-toolkit#personal)
- [Dapp development](https://medium.com/coinmonks/developing-ethereum-dapps-with-truffle-ganache-and-metamask-31bc5023ce91) with Metamask, Ganache and Truffle.
- [Create smart contract](https://www.codeooze.com/blockchain/ethereum-truffle-hello-world/) for Ethereum.
- [Blockchain learning path](https://github.com/protofire/blockchain-learning-path)
- Introduction to [Ganache](https://www.codementor.io/swader/developing-for-ethereum-getting-started-with-ganache-l6abwh62j).
- [ Smart contracts with Truffle](https://blog.abuiles.com/blog/2017/07/08/writing-smart-contracts-with-truffle/).
