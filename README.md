# Da Nonna Peppa — pubblicazione online

Questo è un progetto pronto per essere messo online, così puoi verificare
i pulsanti che nell'anteprima di qui potrebbero essere bloccati (upload
documento, invio email automatico, WhatsApp/email diretti).

## La via più semplice: GitHub + Vercel (nessuna installazione sul computer)

1. Vai su **github.com**, crea un account gratuito se non l'hai già
2. Crea un nuovo repository (es. "da-nonna-peppa"), pubblico o privato
3. Carica dentro tutti i file di questa cartella (trascinali nella pagina
   "Add file" → "Upload files" sul sito di GitHub — non serve la riga di
   comando)
4. Vai su **vercel.com**, crea un account gratuito collegandoti con GitHub
5. Clicca "Add New" → "Project", scegli il repository appena creato
6. Vercel riconosce automaticamente che è un progetto Vite: lascia le
   impostazioni di default e clicca "Deploy"
7. Dopo circa un minuto ottieni un link vero, tipo
   `da-nonna-peppa.vercel.app` — aprilo e testa tutto

Ogni volta che vuoi aggiornare l'app: carichi i nuovi file su GitHub
(sostituendo `src/App.jsx`), e Vercel ripubblica automaticamente in
pochi secondi.

## Alternativa: Netlify

Stessa procedura ma su **netlify.com** — dopo aver collegato GitHub,
Netlify chiede "Build command" (scrivi `npm run build`) e
"Publish directory" (scrivi `dist`).

## Cosa testare una volta online

- Upload del documento d'identità nel form di prenotazione
- Invio automatico dell'email di conferma/rifiuto (EmailJS)
- Pulsanti WhatsApp/Email diretti (oltre a "Copia messaggio")
- Notifiche del browser quando arriva una richiesta

## File di questo progetto

- `src/App.jsx` — tutta l'app (identica a quella che stai già usando qui)
- `src/main.jsx` — punto d'ingresso React
- `index.html`, `package.json`, `vite.config.js` — impalcatura del progetto

Non serve installare nulla sul tuo computer per pubblicarla: tutto il
lavoro di compilazione lo fa Vercel/Netlify quando carichi i file.
