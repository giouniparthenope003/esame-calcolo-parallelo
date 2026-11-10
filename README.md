# Esame di Calcolo Parallelo e Distribuito

Materiale di preparazione all'esame orale di **Calcolo Parallelo e Distribuito** (9 CFU, Prof.ssa L. Marcellino, Università Parthenope).

- **Esame orale:** 27 novembre 2026. Lo scritto è già superato.
- **Obiettivo:** migliorare l'esposizione formale e i concetti teorici, con le definizioni, le derivazioni e i trade-off architetturali richiesti all'orale.

## Contenuto

### Dispense di ripasso

| File | Argomento |
|---|---|
| `01_Fondamenti.pdf` | Motivazioni del calcolo parallelo, T₁ e Tₚ, speed-up, efficienza, overhead, legge di Ware-Amdahl. Include le derivazioni passo passo con il riferimento alla slide, le verifiche numeriche delle discrepanze con le slide e un box "Come esporlo all'orale". |

### Slide delle lezioni

| Blocco | File |
|---|---|
| Introduzione e architetture | `Lez1_intro_motivazioni`, `Lez2_Flynn`, `Lez2_PD_introOpenMP`, `Lez3_intro_MULTICORE_openMP`, `Lez4_decomposizionePROB_multicore`, `Lez4_decPROB_multicore` |
| Parametri di valutazione | `Lez6_intro_Efficienza`, `Lez7_Efficienza_WA`, `Lez10_IsoefficienzaScalabilita_contiSOMME1`, `Lez11_WAgeneralizzata_contiSOMME2`, `Lez11_Lez11_conti_sommaVETT_sommaNnumeri` |
| Prodotto scalare e convoluzione | `Lez13_prodotto_scalare`, `Lez13_ProdottoScalare_parallelo`, `Lez16_convoluzione_1D` |
| Ricerca e ordinamento (seminario) | `Lez15_seminario_Ricerca_Ordinamento_parallelo`, `17 Lezione_seminario_Ricerca_Ordinamento_parallelo` |
| Matrici | `Lez18_MATRICI_fullPARALLEL`, `Lez19_confronti_strategieFULLparallel_2D` |
| Prodotto matrice-vettore | `Lez21_MatVet_intro_conti1strategia`, `Lez23_MatVet_conti2strategia`, `Lez25_MatVet_conti3strategia`, `Lez27_MatVet_finale_MATLAB` |
| Laboratori OpenMP | `Lez5_laboratorio1` … `Lez26_Laboratorio10_openMP_provaSCRITTA_tipo` |

Altro materiale:
- `Formulario Complessità.pdf`: T₁ e Tₚ di tutti gli algoritmi del corso.
- `Teoria Calcolo Parallelo (1).pdf`: appunti di teoria.
- `Esercizi Esame Calcolo Parallelo/`: foto di tracce d'esame, da usare nelle simulazioni.

Alcune lezioni compaiono in due versioni, ad esempio `Lez6_intro_Efficienza.pdf` e `Lez6_intro_Efficienza (1).pdf`.

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
