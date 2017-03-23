# Introduzione

Il progetto consiste nel monitorare in remoto opere d'Arte attraverso l'utilizzo di sensori e microcontrollori.

## Scopo

Un esempio concreto potrebbe essere un'infiltrazione all'interno del tetto di una chiesa. Essa potrebbe causare dei danneggiamenti più o meno gravi al patrimonio artistico di quest'ultima. I danni causati potrebbero non essere notati e aggraversi nel corso del tempo. Il nostro scopo è segnalare tempestivamente un'eventuale anomalia al fine di risolvere immediatamente il problema.

## Specifiche tecniche

### Strumentazione 

 * Microcontrollore - Arduino
 * Singleboard Computer - Lattepanda o Raspberry Pi

### Cosa dobbiamo misurare?

 * Temperatura - Range(0°C - 27°C)
 * Pressione - Range(X hPa - Y hPa)
 * Umidità - Range(X kg/cm^3 - Y kg/cm^3)
 * Luce - Range(X cd - Y cd)

### Come lo dobbiamo misurare?

| Fattore        | Sensore           |
| ------------- |:-------------:|
| Temperatura     | Termoresistenza |
| Pressione      | Mems      |
| Umidità | Mems      |
| Luce | Fotoresistenza & Sensore per lunghezza d'onda     |

### Quando lo dobbiamo misuare?

Considerando che possediamo 4 fattori, ognuno dei quali genera un 1 byte, supponendo di fare 3 misurazioni all'ora per 25 opere in una pinacoteca qualsiasi, in un giorno produremmo 7 Kilobyte corrispondenti a poco meno di 3 Megabyte in un anno.
