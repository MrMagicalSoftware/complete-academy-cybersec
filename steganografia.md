# Steganografia



Steghide è uno strumento di steganografia che consente di nascondere dati all'interno di file multimediali, come immagini e audio. 

![gg](https://github.com/user-attachments/assets/d893553d-28b6-4473-9b14-3ba8a0a503af)




### Installazione
Puoi installare Steghide su sistemi basati su Linux utilizzando il gestore di pacchetti.


```bash
sudo apt-get install steghide
```

### Utilizzo di base

1. **Nascondere un file**:
   Per nascondere un file (ad esempio, un documento di testo) all'interno di un'immagine, usa il comando:

   ```bash
   steghide embed -cf immagine.jpg -ef file_da_nascondere.txt
   ```

   Qui `-cf` specifica il file contenitore (l'immagine) e `-ef` specifica il file da nascondere.

2. **Estrazione di un file**:
   Per estrarre il file nascosto dall'immagine, usa il comando:

   ```bash
   steghide extract -sf immagine.jpg
   ```

   Ti verrà chiesto di inserire la password se ne hai impostata una durante l'inserimento.

3. **Opzioni aggiuntive**:
   - Puoi specificare una password durante l'inserimento con l'opzione `-p`:
     ```bash
     steghide embed -cf immagine.jpg -ef file_da_nascondere.txt -p tua_password
     ```
   - Per visualizzare le opzioni disponibili, puoi usare:
     ```bash
     steghide --help
     ```

### Considerazioni
- utilizzare formati di file supportati (JPEG, BMP, WAV, etc.).
- La steganografia non è una forma di crittografia; è importante proteggere i file nascosti con password se la sicurezza è una preoccupazione.





