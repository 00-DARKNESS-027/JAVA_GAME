
# JavaGame

Gioco 2D multiplayer scritto in Java, con supporto sia per il gioco in locale che online (fino a 2 giocatori).  
Include gestione mappe, NPC, oggetti, cutscene, musica ed effetti sonori.

## Caratteristiche

- Grafica 2D tile-based
- Multiplayer online (2 giocatori, server-client)
- Mappe multiple e oggetti interattivi
- NPC e cutscene
- Musica ed effetti sonori
- Sistema di salvataggio configurazione

## Requisiti

- Java 17 o superiore
- Maven

## Come avviare il gioco

1. **Clona il repository:**
   ```sh
   git clone https://github.com/tuo-username/JavaGameFinal.git
   cd JavaGameFinal
   ```

2. **Compila il progetto:**
   ```sh
   mvn clean package
   ```

3. **Avvia il server (per il multiplayer):**
   ```sh
   java -cp target/JavaGameFinal-1.0-SNAPSHOT.jar network.GameServer
   ```
   Il server ascolta di default su porta 8080. Puoi modificare IP/porta nel codice se necessario.

4. **Avvia il client (giocatore):**
   ```sh
   java -cp target/JavaGameFinal-1.0-SNAPSHOT.jar Main.Main
   ```
   Segui le istruzioni a schermo per collegarti in locale o online.

## Modalità multiplayer

- Solo 2 giocatori possono essere connessi contemporaneamente.
- Se un giocatore si disconnette, lo slot viene liberato e può rientrare.
- Le posizioni dei giocatori vengono sincronizzate in tempo reale.

## Contribuire

1. Fai un fork del progetto
2. Crea un branch per la tua feature/fix
3. Manda una pull request

Sono benvenuti miglioramenti a grafica, gameplay, networking, bugfix e nuove feature!

**Nota:**  
Per problemi o suggerimenti, apri una issue su GitHub.  
Per domande tecniche, consulta i commenti nel codice sorgente.
