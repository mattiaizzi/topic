# BPMN Simulator(WORK IN PROGRESS)
Questo progetto permette di inviare messaggi su un topic ROS e sottoscriversi ad essi attraverso dei diagrammi BPMN.

 - [Installazione](#Installazione)
 - [Utilizzo](#Utilizzo)
 - [Esempi](#Esempi)
 - [Problemi noti](#Problemi noti)

## Installazione <a name="section"></a>
Per installare il progetto è necessario docker.
Comandi git submodule update --init, docker-compose up --build
## Utilizzo
Prima di utilizzare il simulatore è necessarrio avviare [ros2-web-bridge](https://mattia-izzi.gitbook.io/ros2-web-bridge-config/) e assicurasi che apra un web-socket sulla porta 9090
# Esempi

# Problemi noti
Quando viene cambiato il diagramma, si effettuano le sottiscrizioni a tutti i topic, ma non è possibile identificare le singole sottoscrizioni, quindi se nella sezione di esempio mi sono collegato al topic "/example_topic" e nel diagramma anche ho effettuato questa sottoscrizione, verranno eliminate entrambe e la sezione di test non sarà più funzionante
