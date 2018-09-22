# Descripcion UML taller 1 Ecosistemas de Aplicaciones

## Uml servidor en eclipse

### Main
- **main(String[]):void:** Con este metodo se ejecuta la aplicacion
- **Settings():void:** Se usa para definir el tamaño de la aplicacion
- **Setup():void:** Aqui se definen todas las cosas que se ejecutan al iniciar el codigo
- **Draw():void:** Este metodo recibe todo lo que se pintara en pantalla ciclicamente
- **MousePressed():void:** Este metodo permite realizar las acciones que se realizaran con el mouse

### Logica
- **Logica(PApplet) : void:** Construcctor de la logica
- **pintar():void:** Este metodo se utiliza para dibujar recibir todos los metodos 
- **newEnemigo():void:** Este metodo es el que genera Objetos de tipo enemigo conforme avanza el tiempo de la partida
- **impacto():void:** Este metodo es el que valida el impacto de las balas con un enemigo o alguno de los personajes

### Ojetos
+ **Objetos(PApplet, int, int) : void:** Construcctor de los objetos
+ **mover (int,int):void:** Este metodo se utiliza para realizar el cambio en la posicion del personaje, enemigo o recogible
+ **getPosicionX():float:** Se obtiene la posicion horizontal del objeto
+ **setPosicionX(float):void:** Se cambia la posicion horizontal del objeto
+ **getPosicionY():float:** Se obtiene la posicion vertical del objeto
+ **setPosicionY(float):void:** Se obtiene la posicion horizontal del objeto
+ **isMove():boolean:** Se detecta si el objeto esta en movimiento
+ **setMove(boolean):void:** Se determina si el objeto se mueve o no
+ **getVidas() : void:** Se obtiene el numero de vidas que tiene el objeto en cuestion
+ **setVidas(int) : void:** Se cambia el numero de vidas que tiene le objeto en cuestion
+ **getVivo() : void:** Se detecta si el objeto a perdido todas sus vidas o sigue activo
+ **setVivo(boolean) : void:** Se determina si el objeto deja de estar activo o no

### Servidor
+ **run():void:** Es el hilo por el cual se establece la conexion con los clientes
+ **enviar () : void** Envia los datos obtenidos por los botones al servidor 

### Receptor
+ **Receptor(Socket ) : void:** Construcctor del receptor
+ **run():void:** Es el hilo por el cual se reciben los mensajes por parte de los clientes

### Jugador1 
+ **Jugador1(PApplet, int, int) : void:** Construcctor del jugador1
+ **pintar():void:** En este metodo se crean las formas y/o imagenes que compone al jugador
+ **mover():void:** En este metodo se general el cambio de posicion 
+ **gravedad():void:** En este metodo cambia la posicion del jugador al tocar los bordes de la pantalla
+ **disparar(): void:** Aqui se determina que el jugador realiza la animacion para disparar

### Jugador2
+ **Jugador2(PApplet, int, int) : void:** Construcctor del jugador2
+ **pintar():void:** En este metodo se crean las formas y/o imagenes que compone al jugador
+ **mover():void:** En este metodo se general el cambio de posicion 
+ **gravedad():void:** En este metodo cambia la posicion del jugador al tocar los bordes de la pantalla
+ **disparar(): void:** Aqui se determina que el jugador realiza la animacion para disparar

### Enemigo1 
+ **Enemigo1(PApplet, int, int) : void:** Construcctor del enemigo1
+ **pintar():void:** En este metodo se crean las formas y/o imagenes que compone al enemigo
+ **mover():void:** En este metodo se general el cambio de posicion 
+ **gravedad():void:** En este metodo cambia la posicion del enemigo al tocar los bordes de la pantalla
+ **disparar(): void:** Aqui se determina que el enemigo realiza la animacion para disparar

### Enemigo2 
+ **Enemigo2(PApplet, int, int) : void:** Construcctor del enemigo2
+ **pintar():void:** En este metodo se crean las formas y/o imagenes que compone al enemigo
+ **mover():void:** En este metodo se general el cambio de posicion 
+ **gravedad():void:** En este metodo cambia la posicion del enemigo al tocar los bordes de la pantalla
+ **disparar(): void:** Aqui se determina que el enemigo realiza la animacion para disparar

### Bala 
+ **Bala(PApplet, int, int) : void:** Construcctor de la bala
+ **pintar():void:** En este metodo se crean las formas y/o imagenes que componen la bala
+ **mover():void:** En este metodo se general el cambio de posicion 

### Corazon 
+ **Corazon(PApplet, int, int) : void:** Construcctor del corazon
+ **pintar():void:** En este metodo se crean las formas y/o imagenes que componen los corazones
+ **mover():void:** En este metodo se general el cambio de posicion 

### Diamante
+ **Diamante(PApplet, int, int) : void:** Construcctor del diamante
+ **pintar():void:** En este metodo se crean las formas y/o imagenes que componen los diamantes
+ **mover():void:** En este metodo se general el cambio de posicion 

### Estrella 
+ **Estrella(PApplet, int, int) : void:** Construcctor de la estrella
+ **pintar():void:** En este metodo se crean las formas y/o imagenes que componen las estrellas
+ **mover():void:** En este metodo se general el cambio de posicion 


## Uml cliente en android studio

### Main
+ **main (String[] ): void:** Con este metodo se ejecuta la aplicacion
+ **Botones () : void** Con este metodo se detectan las acciones de los botones

### Cliente
+ **Cliente(PApplet, int, int) : void:** Construcctor del cliente
+ **run ( ):** Recibe los datos enviados por parte del servidor
+ **enviar () : void** Envia los datos obtenidos por los botones al servidor 

### Receptor
+ **Receptor(Socket ) : void:** Construcctor del receptor
+ **run ( ):** Recibe los datos enviados por parte del servidor
+ **enviar () : void** Envia los datos obtenidos por los botones al servidor 
