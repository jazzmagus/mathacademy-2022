---
title: 5. Monomi e Polinomi
linktitle: Capitolo 5 monomi e polinomi
abstract: "Il calcolo letterale cambia cmpletamente la prospettiva con la quale guardiamo al calcolo..."
toc: true
type: docs
date: "2019-05-05T00:00:00+01:00"
draft: false
slides: capitolo5
menu:
  math-01:
    parent: 
    weight: 

# Prev/next pager order (if `docs_section_pager` enabled in `params.toml`)
weight: 50
---

{{< toc >}}

> ☆ **scadenza**: 30 marzo 2022

![ex2_img](../ex2_img.png)

Iniziamo oggi un viaggio in un mondo che ci farà vedere la matematica un po' più vicina alla realtà, in quanto

- In alcuni contesti utilizzare dei simboli per indicare generici elementi di un insieme aiuta ad esprimere delle caratteristiche di intere classi di elementi, non singoli oggetti.
- Questo è uno degli aspetti più caratteristici della matematica, occuparsi di fare scoperte e ricavare proprietà su intere categorie di oggetti, nel nostro caso numeri, piuttosto che sui singoli.
- Questo bisogno di generalizzare non è sentito solo in matematica, è simile a ciò che succede in molti contesti quotidiani.

><h4>esempio 1</h4>
>
>se diciamo:
>
><span style="color:orange">Un qualunque individuo minorenne trovato alla guida di un’auto sta commettendo reato.</em></span>
>
>- non ci interessa affatto sapere se tale individuo si chiama Andrea o Giovanni, se è biondo o castano, o se l’auto è una FIAT Panda o una Lamborghini.
>- Ciò che ci interessa è che il soggetto in questione è un **individuo** (cioè un elemento dell’insieme delle persone) minorenne (un elemento dell’insieme delle persone che non ha ancora raggiunto i 18 anni di età) e che si trova alla guida di un auto (un elemento dell’insieme di quei particolari mezzi di trasporto che sono le automobili).
>
><h4>esempio 2</h4>
>
>- se vogliamo rimanere in ambito matematico, pensiamo alle figure geometriche:
>
> - **Area del rettangolo**: <span style="color:orange">$A = a \times b$</span>, con $a$ e $b$, base e altezza;
>   - d'ora in poi sarà molto meglio usare il simbolo "$\cdot$" al posto di "$\times$" per indicare la moltiplicazione, proprio perché utilizzeremo spesso la lettere $x$ e si rischierebbe di confonderla.
> - **Area del quadrato**: <span style="color:orange">$A = l^2$</span>, con $l$ lato del quadrato;
> - **Area del cerchio**: <span style="color:orange">$A_c = 2\pi \cdot r^2$</span>;
>   - questo $2\pi \cdot r^2$ è proprio quello che tra poco chiameremo **monomio**

---

<h2>introduzione</h2>

- Innanzitutto, <mark>che tipo di operazione compiamo quando utilizziamo il calcolo letterale?</mark>
  - Con il **calcolo letterale** si utilizzano dei **simboli** (usualmente lettere) al posto degli **elementi di un insieme** (di solito insiemi numerici), per sottolineare che non stiamo indicando nessun elemento in particolare, ma uno generico. 
  - Stiamo perciò facendo un’affermazione che vale contemporaneamente per tutti gli elementi di un insieme, non di un solo elemento specifico. 

<h3>Utilità del Calcolo Letterale:</h3>

- In alcune occasioni sostituire simboli ai numeri aiuta a semplificare i conti. 
- Sostituire a dei numeri un'unica semplice lettera può permettere di svolgere molti calcoli simili una volta sola, oppure evitare di dover effettuare conti con numeri di molte cifre.

1. Se si devono effettuare molti calcoli dalla stessa struttura, ma con numeri diversi, è utile fare i calcoli una volta sola, sostituendo ai numeri un simbolo, e poi sostituire ai simboli i numeri, così da ottenere i risultati voluti.
2. Ma oltre a questo vantaggio, _sostituire lettere a numeri permette di compiere dei conti e arrivare a dei risultati che valgono per un’intera classe di elementi_, e non per uno solo.
3. Un particolare pregio del calcolo letterale è poi quello di non dover utilizzare la calcolatrice. Infatti, evitare di svolgere ogni possibile conto numerico immettendo i dati in un calcolatore elettronico può, in alcune occasioni, <mark> far risparmiare molto tempo, evitare errori e aiutare a comprendere a fondo la situazione che si sta trattando.</mark>
4. <b>Il calcolo letterale permette, quindi, di risolvere problemi tra loro simili, una sola volta.</b>

---

<h2>Alcune importanti definizioni:</h2>

{{% callout note %}}

**definizione**: <em>una **espressione algebrica** è una scrittura in cui compaiono sia numeri che lettere, (eventualmente parentesi), legati tra loro da simboli di operazioni matematiche.</em>

- Un’**espressione letterale** o **espressione algebrica** è uno schema di calcolo in cui compaiono numeri e lettere legati dai simboli delle operazioni.
- un'espressione algebrica si dice **razionale** quando le operazioni che compaiono sono quelle di: **addizione**, **sottrazione**, **moltiplicazione** ed **elevamento a potenza**: $$x^2 + y^3$$
- Tra le espressioni algebriche razionali abbiamo quelle **frazionarie**, in cui si ha un'espressione algebrica al numeratore e una al denominatore: $$\dfrac{3x^2}{2x^2 -3y}$$
- Quando invece compare anche la radice allora si parla di espressione algebrica **irrazionale**: $$\sqrt{\dfrac{3x^2}{2x^2 -3y}}$$

{{% /callout %}}

- Il **valore numerico** di un'espressione algebrica si ottiene semplicemente sostituendo alle lettere un numero reale: l'espressione algebrica si trasforma in un'espressione numerica, che assume quindi un valore numerico.
- In un’espressione letterale le lettere rappresentano delle **variabili**, che assumono un preciso significato ==solo== quando vengono sostituite da numeri
  - $2x^2 - 3x + 4$ è un'espressione algebrica
  - se assegnamo ad $x$ il valore $-1$, l'espressione assumerà il valore: $2 \cdot (1)^2 - 3 \dot (1) + 4 = 2 - 3 + 4 = +3 \Rightarrow 3$
  - se invece $x = -1$ otteniamo: $2 \cdot (-1)^2 - 3 \dot (-1) + 4 = 2 + 3 + 4 = +11 \Rightarrow 11$

---

<h2>Monomi</h2>

{{% callout note %}}

>**definizione**:
><span style="color:red">Un **monomio** è una espressione algebrica nella quale:</span>
>
>- compaiono soltanto operazioni di **moltiplicazione** ed **elevamento a potenza**;
>- Gli esponenti delle variabili sono **numeri naturali**, qundi $\in \mathbb{N}$
>
>- sono monomi:
>$7x^3yz^4 \qquad - \dfrac {1}{2} a^2bc^4 \qquad 3a(-2)ab^3 \qquad \sqrt{2}st^2 \qquad v = \dfrac{s}{t}$
>- non sono monomi:
>$7x^3yz^{-4} \qquad - \dfrac {1}{2} a^2bc^4 + \dfrac{5}{6}a^2c\qquad 3 \dfrac{a}{b^3} \qquad 2 \sqrt{s}$

{{% /callout %}}

<h4>Grado complessivo di un monomio</h4>

{{% callout alert %}}

>**definizione**:<br>
><span style="color:orange">Dato un monomio non nullo, si definisce **grado** (o **grado complessivo**) del monomio la somma degli esponenti di tutte le lettere che vi compaiono.</span>

{{% /callout %}}

<h4>Grado di un monomio rispetto ad una variabile:</h4>

{{% callout alert %}}

>**definizione**:<br>
><span style="color:orange">Dato un monomio non nullo, si definisce **grado** del monomio **rispetto ad una lettera**, l'esponente con cui compare quella lettera all'interno del monomio, una volta ridotto in **forma normale**</span>
>
>- il monomio: $7x^3yz^4$
>- è di grado $3$ rispetto a $x$, di grado $1$ rispetto a $y$ e di grado $4$ rispetto a $z$.

{{% /callout %}}

---

<h2>Proprietà e operazioni con i monomi:</h2>

>**nota**:<br><em>In una espressione algebrica il punto utilizzato per indicare l'operazione di moltiplicazione viene spesso omesso, quindi l'espressione algebrica $xyz^2$ ha il significato di $x \cdot y \cdot z^2$.</em>
>
>Un monomio si dice **ridotto in forma normale** quando è scritto come prodotto di **un solo** fattore numerico, detto **coefficiente numerico**, e di potenze letterali con basi diverse. Il complesso delle lettere che compaiono nel monomio ridotto a forma normale ne costituisce la **parte letterale**.

<h3>Operazioni con i monomi</h3>

<h4>Somma algebrica di monomi:</h4>

- i monomi devono essere **simili** per poter essere sommati algebricamente:
  - $$3xy^2 - 8xy^2 + xy^2$$
  - $$- \dfrac{1}{2}a^2b + \dfrac{2}{3}a^2b$$
  - $$- 6x + 5x^2y + 4x - 3x^2y$$

<h4>Prodotto tra monomi</h4>

- si sommano gli esponenti: $$(6xy^3z^2) \cdot (- \dfrac{1}{3}y^2z) = -2xy^5z^3$$

<h4>Elevamento a potenza</h4>

- si **moltiplicano** gli esponenti, come per le potenze numeriche:
  - $$\{[(-2a^2b)^2]^3\}^2$$

><h3>Generalizzando</h3>
>
>- Se voglio comprare delle scarpe che costano $50$ euro e sono scontate del $12$%, mi interessa scoprire quanto devo pagare, non fare conti astratti.
>- Ma se sono un commerciante che ogni anno vende un certo numero di paia di scarpe, e devo calcolare quali sconti fare per avere un certo guadagno e aumentare le vendite, è piú utile che egli faccia dei conti riapplicabili in ogni occasione, anziché perdere tempo a ripetere gli stessi procedimenti ogni volta.

---

<h2>Polinomi</h2>

{{% callout alert %}}

>**definizione**:<br>
><span style="color:orange">**definizione**: Un **polinomio** è una **somma algebrica** di **monomi**, non simili.</span>

{{% /callout %}}

**sono polinomi:** $6a + 2b; \quad 5a^2b + 3b^2; \quad 6x^2 - 5y^2x - 1; \quad 7ab - 2a^2b^3 + 4$.

*osserva che*:

- Se tra i termini di un polinomio non sono presenti monomi simili, il polinomio si dice in forma **normale** o **ridotto**;
- se al contrario si presentano dei termini simili, possiamo eseguire la riduzione del polinomio sommando i termini simili.
- Tutti i polinomi sono quindi riducibili in forma normale.
- Un polinomio in forma normale può presentare tra i suoi termini un monomio di grado $0$ che viene comunemente chiamato **termine noto**.

---

<h4>grado di un polinomio</h4>

> **definizione**:<br> Il **grado complessivo** (o semplicemente grado) di un polinomio è il massimo dei gradi complessivi dei suoi termini. Si chiama, invece, grado di un polinomio rispetto ad una data lettera l’esponente maggiore con cui quella lettera compare nel polinomio, dopo che è stato ridotto a forma normale.
>
>- Il polinomio $2ab + 3 - 4a^2b^2$ ha grado complessivo $4$ perché il monomio con grado massimo è $- 4a^2b^2$, che è un monomio di quarto grado;
>
>- il grado del polinomio $a^3 + 3b^2a - 4ba^2$ rispetto alla lettera $a$ è $3$ perché l’esponente più grande con cui tale lettera compare è $3$.

- Un polinomio si dice **omogeneo** se tutti i termini che lo compongono sono dello *stesso grado*.

- Un polinomio si dice **ordinato secondo le potenze decrescenti (*crescenti*) di una lettera**, quando i suoi termini sono ordinati in maniera tale che gli esponenti di tale lettera decrescono (*crescono*), leggendo il polinomio da sinistra verso destra.

- Un polinomio di grado $n$ rispetto ad una data lettera si dice **completo** se contiene tutte le potenze di tale lettera di grado inferiore a $n$, compreso il termine noto.

---
## Proprietà dei polinomi

## Operazioni con i polinomi

## somma algebrica e "differenza"

> La somma algebrica comprende anche la "sottrazione", che nel Calcolo Letterale viene interpretata come una **somma algebrica** con l'**opposto** del polinomio da sottrarre.

## prodotto di un monomio per un polinomio

- Si esegue moltiplicando il monomio per ognuno dei termini del polinomio, sommando algebricamente i monomi risultanti
- Il prodotto tra un monomio e un polinomio è certamente un **caso particolare** del prodotto tra polinomi in quanto un monomio può essere pensato come un caso particolare di polinomio, composto di un solo termine.
- **esempio**:

## prodotto di polinomi

## quoziente di un polinomio e un monomio

## Prodotti Notevoli

## Divisione tra polinomi

## esempi

## conclusioni
