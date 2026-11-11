# Le 3 skill che danno gusto a Claude Code: guida di Studio Beezy

> **Per chi legge:** non devi fare niente a mano. Apri Claude Code nella cartella del tuo progetto,
> dagli questo file (o il suo link) e scrivi: **«segui questa guida»**.
>
> **Per Claude:** questa guida è scritta per te. Esegui i passi in ordine, uno alla volta, e
> spiega in italiano semplice cosa stai facendo. Prima di ogni installazione di' cosa installi e
> da dove, e aspetta l'ok della persona. Non installare nient'altro oltre a quello che c'è qui.

Comandi verificati sui README ufficiali l'11 novembre 2026. Se un comando è cambiato, vale il README
del repository, non questa guida: leggilo e dillo alla persona.

## 0. Controlli prima di partire

1. Lancia `node --version`. Serve **Node 22 o più recente**. Se manca o è più vecchio, fermati e
   spiega come installarlo da nodejs.org: non proseguire.
2. Controlla che sul computer ci sia Chrome, Edge o Chromium (serve a Taste Skill per guardare le pagine).
3. Chiedi alla persona: **«Le vuoi solo in questo progetto o in tutti i tuoi progetti?»**
   e usa la risposta in ogni installazione qui sotto.

I comandi `npx skills add` fanno domande a schermo. Per rispondere da riga di comando aggiungi:
`-a claude-code` (installa per Claude Code), `-y` (salta le conferme) e, solo se la persona le
vuole in tutti i progetti, `-g`. Senza `-g` finiscono nel progetto corrente.
Se un comando si ferma lo stesso su una domanda, lancialo con `--help` e riprova con le opzioni giuste.

## 1. Taste Skill: il gusto

Repository: https://github.com/Leonxlnx/taste-skill

```
npx skills add https://github.com/Leonxlnx/taste-skill --skill "design-taste-frontend"
```

Cosa fa: toglie alle pagine i segni tipici dell'AI (stessi caratteri, stesse sfumature viola, stesse
schede tutte uguali). Dà a Claude una direzione artistica, immagini di riferimento e un controllo
nel browser prima di dire «finito».

## 2. Le skill di Emil Kowalski: il movimento

Repository: https://github.com/emilkowalski/skills

```
npx skills@latest add emilkowalski/skills
```

Il pacchetto ne contiene molte: con `-l` le elenchi senza installare, con `-s nome1 nome2` scegli quali.
Installa almeno queste tre e chiedi alla persona se vuole le altre: `emil-design-eng` (la principale),
`animate` (costruisce un'animazione da zero), `review-animations` (controlla quelle che ci sono già).
Attenzione: anche Impeccable ha un comando che si chiama `animate`. Se dopo il passo 3 i due nomi si
pestano i piedi, dillo alla persona e tieni `emil-design-eng` e `review-animations`.

Cosa fa: le interfacce ferme sembrano piatte. Con queste Claude aggiunge movimento vero: curve
studiate, durate giuste, animazioni che hanno un motivo.

## 3. Impeccable: la rifinitura

Sito: https://impeccable.style · Repository: https://github.com/pbakaus/impeccable

```
npx impeccable install
```

Per rispondere da riga di comando: `--providers=claude` e `--scope=project` oppure `--scope=global`.
L'installatore propone anche un **controllo automatico** che guarda ogni file di interfaccia che
modifichi: spiega alla persona cos'è e chiedile se lo vuole, non deciderlo tu.

Cosa fa: un vocabolario di design completo (caratteri, colori, spazi, impaginazione) dato a Claude
in un colpo solo, con comandi come `/polish`, `/critique` e `/audit`.

## 4. Verifica

1. Di' alla persona di **chiudere e riaprire Claude Code**: le skill nuove si caricano all'avvio.
2. Alla riapertura, controlla che le tre skill compaiano nell'elenco di quelle disponibili.
3. Se una manca, rileggi l'uscita del suo comando di installazione e sistemala prima di andare avanti.

## 5. Prima prova (fagliela fare subito)

Proponi alla persona questi tre passi su una pagina vera del suo progetto:

1. **«Rifai questa pagina con Taste Skill»**: guarda prima e dopo.
2. **«Aggiungi movimento dove serve, e dimmi anche dove NON serve»**: con le skill di Emil.
3. **`/polish`** prima di pubblicare: Impeccable ripassa tutto e sistema i dettagli.

Regola d'oro da dire alla persona: le skill non sostituiscono le idee. Più sai dire cosa vuoi
(per chi è il sito, che aria deve avere, un sito che ti piace), più il risultato è tuo.

---

Fatta da **Studio Beezy**: siti, strumenti e automazioni per chi lavora. studiobeezy.com
Su Instagram ogni settimana strumenti come questi: @studio.beezy
