# Esame di Calcolo Parallelo e Distribuito

Materiale di preparazione all'esame orale di **Calcolo Parallelo e Distribuito** (9 CFU, Prof.ssa L. Marcellino, Università Parthenope).

- **Esame orale:** 27 novembre 2026. Lo scritto è già superato.
- **Obiettivo:** migliorare l'esposizione formale e i concetti teorici, con le definizioni, le derivazioni e i trade-off architetturali richiesti all'orale.

## Contenuto

### Struttura

```
├── CLAUDE.md                   istruzioni di studio, piano e registro progressi
├── README.md
├── Formulario Complessità.pdf  T₁ e Tₚ di tutti gli algoritmi del corso
├── Dispense/                   dispense di ripasso generate
├── Lezioni/                    slide teoriche, LezXX_titolo.pdf (a/b se più file per lezione)
├── Laboratori_OpenMP/          slide dei laboratori
└── Esercizi_esame/             foto di tracce d'esame
```

### Dispense di ripasso (`Dispense/`)

| File | Argomento |
|---|---|
| `01_Fondamenti.pdf` | Motivazioni del calcolo parallelo, T₁ e Tₚ, speed-up, efficienza, overhead, legge di Ware-Amdahl. Include le derivazioni passo passo con il riferimento alla slide, le verifiche numeriche delle discrepanze con le slide e un box "Come esporlo all'orale". |

### Slide delle lezioni (`Lezioni/`)

| Blocco | File |
|---|---|
| Introduzione e architetture | `Lez01_intro_motivazioni`, `Lez02a_Flynn`, `Lez02b_PD_introOpenMP`, `Lez03_intro_MULTICORE_openMP`, `Lez04a_decomposizionePROB_multicore`, `Lez04b_decPROB_multicore` |
| Parametri di valutazione | `Lez06a/b_intro_Efficienza`, `Lez07a/b_Efficienza_WA`, `Lez10_IsoefficienzaScalabilita_contiSOMME1`, `Lez11a_conti_sommaVETT_sommaNnumeri`, `Lez11b_WAgeneralizzata_contiSOMME2` |
| Prodotto scalare e convoluzione | `Lez13a_prodotto_scalare`, `Lez13b_ProdottoScalare_parallelo`, `Lez16_convoluzione_1D` |
| Ricerca e ordinamento (seminari) | `Lez15b_seminario_Ricerca_Ordinamento_parallelo`, `Lez17_seminario_Ricerca_Ordinamento_parallelo` |
| Matrici | `Lez18_MATRICI_fullPARALLEL`, `Lez19_confronti_strategieFULLparallel_2D` |
| Prodotto matrice-vettore | `Lez21_MatVet_intro_conti1strategia`, `Lez23_MatVet_conti2strategia`, `Lez25_MatVet_conti3strategia`, `Lez27_MatVet_finale_MATLAB` |
| Appunti | `Teoria_Calcolo_Parallelo` |

### Laboratori (`Laboratori_OpenMP/`)

`Lez05_laboratorio1`, `Lez08_laboratorio2`, `Lez09_laboratorio3`, `Lez12_laboratorio4`, `Lez14_laboratorio5`, `Lez15a_Laboratorio6`, `Lez20_Laboratorio7`, `Lez22_Laboratorio8`, `Lez24_Laboratorio9`, `Lez26_Laboratorio10_openMP_provaSCRITTA_tipo`.

Le versioni a/b di Lez06 e Lez07 hanno contenuto diverso; la versione "a" è quella usata per le dispense.

## Metodo di studio

La preparazione segue le regole di `CLAUDE.md`, usato come istruzioni per Claude Code nel ruolo di professore:

- per ogni concetto si vedono l'intuizione, la definizione formale e i trade-off;
- per ogni formula si mostra la derivazione passo passo, citando lezione e slide; i passaggi assenti dalle slide sono segnalati come "derivazione mia";
- per ogni algoritmo si percorre la catena **decomposizione → T₁ e Tₚ → Sₚ → Eₚ → isoefficienza/scalabilità → trade-off**;
- le simulazioni d'esame prevedono una domanda alla volta, con voto in trentesimi.

Il **piano di studio** (10–26 novembre) e il **registro dei progressi** (argomenti, voti, errori ricorrenti) sono in [`CLAUDE.md`](CLAUDE.md). A fine sessione il registro viene aggiornato, poi si fa commit e push.

## Riferimenti

- A. Grama, G. Karypis, V. Kumar, A. Gupta, *Introduction to Parallel Computing*, 2nd ed., Addison Wesley.
- Slide del corso, Prof.ssa L. Marcellino.

> Repository privato a uso personale di studio. Le slide sono materiale didattico del corso e non vanno ridistribuite.
