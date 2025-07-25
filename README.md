


# Work-time - Schedulatore Ore Lavoro

Un'applicazione web progressiva (PWA) per il tracciamento del tempo di lavoro, progettata per aiutarti a monitorare e gestire le tue ore di lavoro su diversi progetti.

## 🚀 Caratteristiche

- **Tracciamento del tempo in tempo reale** - Avvia e ferma il timer per registrare le sessioni di lavoro
- **Gestione progetti** - Crea e organizza diversi progetti di lavoro
- **Statistiche dettagliate** - Visualizza grafici e report sui tuoi tempi di lavoro
- **Note di sessione** - Aggiungi note descrittive per ogni sessione di lavoro
- **Esportazione/Importazione dati** - Backup e restore dei tuoi dati in formato JSON
- **Funziona offline** - PWA con supporto offline tramite service worker
- **Responsive** - Ottimizzato per desktop, tablet e smartphone

## 🛠 Installazione e Utilizzo

### Metodo 1: Server web locale
```bash
# Clona il repository
git clone https://github.com/lellimami/Work-time.git
cd Work-time

# Avvia un server web locale
python3 -m http.server 8000
# oppure
npx serve .

# Apri il browser su http://localhost:8000
```

### Metodo 2: Apertura diretta
Puoi anche aprire direttamente il file `index.html` nel tuo browser, ma alcune funzionalità potrebbero essere limitate.

## 📱 Installazione come PWA

1. Apri l'applicazione nel tuo browser
2. Cerca l'opzione "Installa app" o "Aggiungi alla schermata home"
3. Segui le istruzioni per installare l'app sul tuo dispositivo

## 🎯 Come usare l'applicazione

1. **Crea un progetto**: Clicca su "+ Nuovo Progetto" nella barra laterale
2. **Avvia il timer**: Seleziona un progetto e clicca su "START"
3. **Aggiungi note**: Scrivi note per descrivere cosa stai facendo
4. **Ferma il timer**: Clicca su "STOP" quando hai finito
5. **Visualizza statistiche**: Controlla i grafici e lo storico delle sessioni

## 💾 Gestione dei dati

- I dati sono salvati automaticamente nel browser (localStorage)
- Usa "Esporta Dati (JSON)" per fare backup
- Usa "Importa Dati (JSON)" per ripristinare backup precedenti

## 🔧 Sviluppo

Il progetto è sviluppato con:
- HTML5, CSS3, JavaScript vanilla
- Chart.js per i grafici
- Tailwind CSS per lo styling
- Service Worker per il supporto offline

## 🐛 Risoluzione problemi

**I grafici non si caricano**: L'app funziona anche se le CDN esterne sono bloccate, ma i grafici mostreranno messaggi informativi invece delle visualizzazioni.

**L'app non si installa**: Assicurati di servire l'app tramite HTTPS o localhost per abilitare le funzionalità PWA.

## 📄 Licenza

ISC License - Vedi il file di licenza per i dettagli.
