# MyFoodMind

Zero scarti alimentari: scannerizza gli alimenti che hai in casa, ricevi un promemoria prima della scadenza e ottieni ricette consigliate per usarli in tempo.

Progetto del gruppo per il corso IAL Start Up, area **4 Ristorazione**.

## Idea

1. **Scansione**: l'utente scannerizza gli alimenti (ad esempio il codice a barre o l'etichetta).
2. **Scadenze**: l'app registra la data di scadenza e avvisa quando un alimento sta per scadere.
3. **Ricette**: in base agli alimenti in scadenza, l'app suggerisce ricette per non buttare nulla.

## Stato del progetto

Disponibile una **versione dimostrativa** (`index.html`, pagina unica senza dipendenze), sul branch `app-dimostrativa`:

- **Frigo**: alimenti ordinati per scadenza con colori (verde, arancione, rosso), avviso "Scade presto", pulsanti Consumato / Elimina.
- **Aggiungi**: scansione del codice a barre con la fotocamera (dove il browser lo supporta), codice digitato o inserimento a mano; la scadenza si sceglie dal calendario, con una durata tipica proposta per categoria.
- **Ricette**: 14 ricette abbinate agli alimenti presenti, con priorità a quelli che scadono prima.
- **Anti-spreco**: statistiche su consumati in tempo, scaduti e alimenti nel frigo.

I dati restano salvati solo nel browser del dispositivo (nessun account, nessun server).

### Come provarla

Apri `index.html` in un browser. Per la fotocamera serve una pagina `https://` o `localhost`; senza fotocamera usa i codici d'esempio nella scheda Aggiungi.

### Limiti della demo

- Catalogo di codici a barre minimo (6 codici d'esempio); gli altri codici si cercano su Open Food Facts, se online.
- Nessun avviso push: l'avviso di scadenza compare solo dentro l'app.
- Nessuna sincronizzazione tra dispositivi.

## Come lavorare insieme

```bash
git clone https://github.com/zikoindustris/myfoodmindzikind.git
cd myfoodmindzikind
git pull            # scarica le novità prima di iniziare
# ...modifica i file...
git add .
git commit -m "Descrizione breve della modifica"
git push
```

Consigli: fai `git pull` prima di iniziare a lavorare e scrivi messaggi di commit chiari, così il gruppo capisce cosa è cambiato.

## Team

Aggiungere qui i nomi dei componenti del gruppo.
