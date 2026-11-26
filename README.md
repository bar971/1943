# 1943: Battaglia delle Midway - Arcade Clone

Un clone tributo in formato **one-page app HTML5** del mitico sparatutto arcade a scorrimento verticale **1943: The Battle of Midway**, originariamente sviluppato da **Capcom** e uscito nelle sale giochi nel **1987**.

**Gioca subito dal browser:** [https://bar971.github.io/1943/](https://bar971.github.io/1943/)

## Il gioco originale (1987)

Seguito del celebre *1942* (1984), **1943: The Battle of Midway** è diventato uno dei simboli delle sale giochi anni '80. Ambientato nel teatro del Pacifico durante la Seconda guerra mondiale, mette il giocatore ai comandi di un caccia bimotore americano **Lockheed P-38 Lightning** contro squadriglie aeree e grandi navi da guerra giapponesi, fino allo scontro finale con la corazzata **Yamato**.

Tra le idee che lo resero leggendario:
- **Barra energia/carburante:** scende sia subendo colpi sia col passare del tempo, spingendo a cercare costantemente i rifornimenti `POW`.
- **Potenziamenti selezionabili a colpi di mitragliatrice:** sparando ai `POW` rilasciati dalle squadriglie rosse si può cambiare il tipo di arma o bonus prima di raccoglierlo.
- **Armi temporanee e mosse speciali:** sparo a 3 vie (`3-WAY`), fucile a pompa (`SHOTGUN`, capace di distruggere anche i proiettili nemici), `LASER`, la manovra evasiva **Loop** e l'attacco speciale **Fulmine** che colpisce tutti i nemici sullo schermo consumando energia.

## Caratteristiche di questo clone

- **Unico file HTML autonomo (`index.html`):** zero dipendenze esterne, nessuna installazione richiesta, audio retro generato interamente via **Web Audio API**.
- **Grafica HD vettoriale su Canvas 2D (HiDPI):** gradienti metallici, riflessi, lampi di sparo, onde d'urto, fumo persistente sui boss danneggiati, atmosfere di luce distinte per ogni livello e filtro **CRT** opzionale.
- **3 livelli di difficoltà selezionabili:** `FACILE`, `NORMALE` e `ARCADE`.
- **5 missioni progressive con boss dedicati:**
  1. *Avanguardia del Pacifico* - Boss: **Incrociatore Tone**
  2. *Cieli delle Midway* - Boss: **Portaerei Akagi**
  3. *Tempesta di Fuoco* - Boss: **Incrociatore Kaga**
  4. *Fortezza Volante* - Boss: **Bombardiere Ayako**
  5. *Battaglia Finale* - Boss: **Corazzata Yamato** (con **3 torrette distruttibili** indipendenti)
- **Animazioni di distruzione:** affondamento in mare dei boss navali tra esplosioni a catena e anelli di schiuma, schianto in acqua del bombardiere e caduta in avvitamento del P-38.
- **Salvataggio record locale** tramite `localStorage`.

## Comandi

| Azione | Mouse | Tastiera |
| --- | --- | --- |
| Muovi il P-38 | Movimento sul Canvas | `WASD` o `Frecce` |
| Fuoco | `Click Sinistro` (tieni premuto) | `Spazio` o `Z` |
| Loop (schiva proiettili) | `Click Destro` | `Shift` o `X` |
| Fulmine (-15 Energia) | - | `E` o `C` |
| Pausa | Pulsante UI | `P` |
| Audio On/Off | Pulsante UI | `M` |
| Filtro CRT On/Off | Pulsante UI | `V` |

## Esecuzione in locale

Non serve alcun server o build step: scarica o clona il repository e apri `index.html` direttamente in un browser moderno.

```bash
git clone https://github.com/bar971/1943.git
cd 1943
```

---

*Progetto amatoriale a scopo dimostrativo e di tributo al classico arcade Capcom del 1987.*
