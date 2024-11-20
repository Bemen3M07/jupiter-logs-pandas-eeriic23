[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/ULiw8LbN)
# Empty
Repositori buit


Exercici 2 Punt2
2- Que creieu que és millor mostrar els logs per exemple a la terminal durant l'execució del programa o bolcar-los en un fitxer de text? Afegiu al readme.md
del repositori aquesta pregunta amb la seva reposta

És millor mostrar els logs a la terminal durant el desenvolupament, per facilitar la depuració immediata. En producció, cal emmagatzemar-los en fitxers per assegurar un historial durador i accessible.

Exercici 2 Punt3

| Mètode                                                  | Exemple                                   | Avantatges                                                      | Desavantatges                         |
|---------------------------------------------------------|-------------------------------------------|-----------------------------------------------------------------|-------------------------------------------|
| Configuració per defecte del mòdul `logging`            | `logging.basicConfig(level=logging.INFO)` | Simple i ràpid de configurar.                                   | No és gaire flexible i no permet gestionar   múltiples fitxers.                                      |
| Instanciar un objecte logger i parametritzar-lo         | `logger = logging.getLogger('my_logger')` | Flexibilitat per afegir múltiples handlers, formats i nivells.  | Configuració inicial més complexa, fàcil     cometre errors.                                         |
| Instanciar un objecte logger des d’una configuració     | `logging.config.fileConfig('config.ini')` | Permet configuracions avançades sense modificar el codi.        | Requereix mantenir fitxers de configuració   externs.                                                |




Exercici 2 Punt4

| Característica                    | Python (`logging`)                       | Java (`java.util.logging`)            | Node.js (`winston`)                                    |
|-----------------------------------|------------------------------------------|---------------------------------------|--------------------------------------------------------|
| Nom de la llibreria               | `logging`                                | `java.util.logging`                   | `winston`                                              |
| És nativa del llenguatge?         | Sí                                       | Sí                                    | No (biblioteca externa)                                |
| URL per descarregar-se la llibreria| [logging](https://docs.python.org/3/library/logging.html) | Inclosa al JDK      | [winston](https://github.com/winstonjs/winston)        |
| Inicialització de l'objecte logger | `logging.getLogger()`                    | `Logger.getLogger("nom")`            | `const logger = require('winston');`                   |
| Nivells de log disponibles        | `DEBUG`, `INFO`, `WARNING`, `ERROR`, `CRITICAL` | `FINE`, `INFO`, `WARNING`, `SEVERE`| `error`, `warn`, `info`, `http`, `verbose`, `debug` |
| Mètode per fer log                | `logger.info("msg")`                     | `logger.info("msg")`                  | `logger.log('info', "msg")`                            |
| Tipus de manejadors disponibles   | Pantalla, fitxer                         | Consola, fitxer                       | Consola, fitxer, serveis remots com AWS o MongoDB      |
| Opcions de format                 | `%Y-%m-%d %H:%M:%S`                      | Patrons personalitzats via `Formatter`| JSON, string customitzat, o configuracions de transports|
