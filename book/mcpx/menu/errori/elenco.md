# Elenco errori



## Codice 001 {#001}
Contatto relè di fase aperto.

#### Descrizione
Il relè di fase è presente sui quadri in impianti a fune senza VVVF e oleodinamici. Controlla le fasi della rete di alimentazione. Nel caso di sfasamento, apre un contatto di allarme.

#### Cause
Le fasi della rete in ingresso sono state cambiate o non sono in fase.

#### Soluzioni
Girare le fasi per metterle in fase.

---

## Codice 002 {#002}
Contatto relè termico aperto (impianto a fune 1-2 velocità).

#### Descrizione
Il relè termico è presente in impianti a fune a 1 o 2 velocità e apre un contatto in caso di eccessivo
assorbimento sulla rete della forza motrice.

#### Cause
1. il motore sta lavorando eccessivamente
2. basso isolamento tra gli avvolgimenti

#### Soluzioni
1. controllare che il carico del motore non sia eccessivo
2. controllare isolamento avvolgimenti

Controllare assorbimento del motore sotto carico.

---

## Codice 003 {#003}
Contatto termico olio aperto (impianto oleodinamico).

#### Descrizione
Le centraline oleodinamiche hanno un relè che apre un contatto in caso di surriscaldamento dell'olio.

#### Cause
La centralina sta lavorando eccessivamente

#### Soluzioni
Controllare che il carico della centralina non sia eccessivo

---

## Codice 004 {#004}
Intervento allarme VVVF (impianto a fune).

#### Descrizione
Il VVVF in dotazione sugli impianti a fune ha un uscita di allarme.

#### Cause
Da ricercare nel codice di errore del VVVF.

#### Soluzioni
Da ricercare nel codice di errore del VVVF.

---

## Codice 005 {#005}
Collegamento termistori motore aperto o interrotto.

#### Descrizione
I motori hanno una serie di contatti che si aprono in caso di sovratemperatura su uno o più avvolgimenti.
L'errore segnala che il collegamento è assente.

#### Cause
Cavo interrotto o non collegato.

#### Soluzioni
Controllare collegamento tra termistori e quadro di manovra.

---

## Codice 006 {#006}
Intervento termistori motore per sovratemperatura.

#### Descrizione
I motori hanno una serie di contatti che si aprono in caso di sovratemperatura su uno o più avvolgimenti.
L'errore segnala che la serie si è aperta per sovratemperatura.

#### Cause
1. il motore sta lavorando eccessivamente
2. basso isolamento tra gli avvolgimenti

#### Soluzioni
1. controllare che il carico del motore non sia eccessivo
2. controllare isolamento avvolgimenti

Controllare assorbimento sotto carico.

---

## Codice 007 {#007}
Tensione 48VDC di manovra assente.

#### Descrizione
La tensione di manovra è la tensione di lavoro per il circuito di manovra, ovvero il circuito che monitorizza la serie
di sicurezza e comanda glia componenti del quadro.

#### Cause
Tensione assente all'inizio della catena delle sicurezze.

#### Soluzioni
* controllare l'intervento della valvola di manvovra
* controllare trasformatore di alimentazione del quadro
* controllare circuito alimentazione manvora

---

## Codice 008 {#008}
Contatto extracorsa aperto.

In impianti oleodinamici questo errore provoca il __blocco dell'impianto__ (vedi [blocco per errore di extracorsa](../../blocco_errore/README.md#extracorsa)).

#### Descrizione
L'impianto è andato oltre il limite impostato dell'extracorsa.

#### Cause
La cabina non si è fermata. Potrebbe non essere stato ricevuto il comando di fermata.
Possibili cause sono:
1.   interferenze magnetiche
2.   accoppiamento piste magnetiche e induttori non corretto
3.   induttori difettosi
4.   cavo di cabina rovinato
5.   piste di fermata registrate non correttamente

#### Soluzioni
1.   posizionare le piste di fermata con lati opposti (ad esempio una con lato giall ed una con lato nero)
2.   controllare che la distanza tra induttori e piste non sia maggiore di 1cm
3.   controllare che gli induttori non siano difettosi
4.   controllare che il cavo di cabina non sia interrotto
5.   assicurarsi che lo spazio di sovrapposizione tra le piste di fermata sia di almeno 2cm, regolare la fermata con i parametri [015](../parametri/temporizzazioni.md#015) e [016](../parametri/temporizzazioni.md#016).

---

## Codice 009 {#009}
Contatti 2-3-4 catena sicurezze aperti.
#### Descrizione
La catena dei contatti della serie di sicurezza tra 2 e 4 (morsetti del quadro) è aperta.

#### Cause
L'impianto non era in manutenzione e:
*    si è aperto il contatto di ALT
*    si è aperto il deviatore normale/manovra

#### Soluzioni
Controllare bottoniera di manovra in cabina.

---

## Codice 010 {#010}
Contatti 5-6-7 catena sicurezze aperti.

#### Descrizione
La catena dei contatti della serie di sicurezza tra 5 e 7 (morsetti del quadro) è aperta.

#### Cause
1. intervenuto alt cabina
2. intervenuto cev
3. intervenuto paracadute

#### Soluzioni
1. controllare contatto alt cabina
2. controllare contatto cev
3. controllare contatto paracadute

---

## Codice 011 {#011}
Contatto preliminari aperto durante il viaggio.

#### Descrizione
Il contatto dei preliminari (morsetti 7-8 sulla serie delle sicurezze) si è aperto in viaggio.

#### Cause
1. i contatti delle serrature sono difettosi
2. il cavo di vano è difettoso

#### Soluzioni
1. controllare i contatti delle serrature
2. controllare il cavo di vano

---

## Codice 012 {#012}
Contatto porte cabina aperto durante il viaggio.

#### Descrizione
Il contatto delle porte di cabina (morsetti 8-9 del quadro sulla serie delle sicurezze) si è aperto in viaggio.

#### Cause
1. i contatti delle porte di cabina sono difettosi
2. il cavo di cabina è difettoso

#### Soluzioni
1. controllare i contatti di cabina
2. controllare il cavo di cabina

---

## Codice 013 {#013}
Relè PV attratto in bassa velocità (impianto oleodinamico).

#### Descrizione
È stato ricevuto il comando di rallentamento e il relè PV sarebbe dovuto cadere per chiudere la valvola di livellazione e mandare impianto in bassa velocità.

#### Cause
1. relè difettoso
2. contatto relè di feedback alla scheda difettoso (vedi schema del quadro)
3. ingresso feedback della scheda difettoso (pin 42, vedi [layout](../../layouts/mcpx.md))
4. uscita di comando scheda difettosa (pin 66, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. cambiare il relè
2. cambiare relè
3. 4 mandare scheda in assistenza

---

## Codice 014 {#014}
Teleruttore PV non attratto in bassa velocità (impianto fune a 2 velocità).

#### Descrizione
È stato ricevuto il comando di rallentamento e il teleruttore PV sarebbe dovuto attrarsi (dopo la caduta di P) per comandare la bassa velocità.

#### Cause
1. teruttore difettoso
2. contatto del teleruttore di feedback alla scheda difettoso (vedi schema del quadro)
3. ingresso feedback della scheda difettoso (pin 42, vedi [layout](../../layouts/mcpx.md))
4. uscita di comando scheda difettosa (pin 66, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. cambiare il teleruttore
2. cambiare il contatto o teleruttore
3. 4 mandare scheda in assistenza

---

## Codice 015 {#015}
Teleruttore P attratto in bassa velocità (impianto fune a 2 velocità).

#### Descrizione
È stato ricevuto il comando di bassa velocità e il teleruttore P non è caduto.

#### Cause
1. teruttore difettoso
2. contatto del teleruttore di feedback alla scheda difettoso (vedi schema del quadro)
3. ingresso feedback della scheda difettoso (pin 41, vedi [layout](../../layouts/mcpx.md))
4. uscita di comando scheda difettosa (pin 65, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. cambiare il teleruttore
2. cambiare il contatto o teleruttore
3. 4 mandare scheda in assistenza

---

## Codice 016 {#016}
Pre-finecorsa aperto in discesa.

#### Descrizione
In impianti veloci per ragioni di sicurezza viene usato un contatto aggiuntivo oltre al finecorsa di discesa.
Questo contatto (prefinecorsa) è meccanico e deve aprirsi dopo che si è aperto il finecorsa di discesa e prima della fermata.

#### Cause
1. contatto difettoso
2. cavo di vano difettoso
3. ingresso scheda difettoso (pin 83, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. sostituire contatto
2. controllare cavo di vano
3. mandare scheda in assistenza

---

## Codice 017 {#017}
Contatto blocchi aperto in discesa.

#### Descrizione
Il contatto 9-10 (morsetti del quadro) delle serie di sicurezza si è aperto mentre la cabina viaggiava in discesa.

#### Cause
1. contatto blocchi difettoso
2. ingresso scheda difettoso (pin 6-7, vedi [layout](../../layouts/mcpx.md))
3. cavo di vano difettoso

#### Soluzioni
1. controllare contatto blocchi
2. mandare scheda in assistenza
3. controllare cavo di vano

---

## Codice 018 {#018}
Teleruttore DIS non attratto in discesa.

#### Descrizione
Effettuata partenza in discesa e il teleruttore DIS ([vedi descrizione](./componenti.md#DIS)) non si è attratto.

#### Cause
1. teleruttore difettoso
2. tensione di manovra bassa
3. uscite della scheda difettose (pin 65 e 67, vedi [layout](../../layouts/mcpx.md))
4. ingressi di feedback della scheda difettosi (pin 41 e 40, vedi [layout](../../layouts/mcpx.md))
5. contatto di feedback del teleruttore alla scheda difettoso (vedi schema del quadro)

#### Soluzioni
1. cambiare teleruttore
2. controllare tensione di manovra ad inizio e fine serie durante il funzionamento e identificare il circuito che provoca il calo di tensione
3. 4 mandare scheda in assistenza
5. cambiare contatto o teleruttore

---

## Codice 019 {#019}
Il contatto 8-9 (morsetti del quadro) delle serie di sicurezza si è aperto mentre la cabina viaggiava in discesa.

#### Cause
1. contatto porte cabina difettoso
2. ingresso scheda difettoso (pin 5-6, vedi [layout](../../layouts/mcpx.md))
3. cavo di vano difettoso

#### Soluzioni
1. controllare contatto porte cabina
2. mandare scheda in assistenza
3. controllare cavo di vano

---

## Codice 020 {#020}
Teleruttore SAL attratto in dicesa.

#### Descrizione
È stata effettuata una partenza in discesa e il teleruttore SAL è rimasto attratto.

#### Cause
1. teleruttore difettoso
2. contatto di feedback del teleruttore alla scheda difettoso (vedi schema quadro)
3. ingresso di feedback della scheda difettoso (pin 39, vedi [layout](../../layouts/mcpx.md)))
4. uscita di comando della scheda difettosa (pin 68, vedi [layout](../../layouts/mcpx.md)))

#### Soluzioni
1. cambiare teleruttore
2. cabiare contatto o teleruttore
3. 4 mandare scheda in assistenza

---

## Codice 021 {#021}
Pre-finecorsa aperto in salita.

#### Descrizione
In impianti veloci per ragioni di sicurezza viene usato un contatto aggiuntivo oltre al finecorsa di salita.

#### Cause
1. contatto difettoso
2. cavo di vano difettoso
3. ingresso scheda difettoso (pin 80, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. sostituire contatto
2. controllare cavo di vano
3. mandare scheda in assistenza

---

## Codice 022 {#022}
#### Descrizione
Il contatto 9-10 (morsetti del quadro) delle serie di sicurezza si è aperto mentre la cabina viaggiava in salita.

#### Cause
1. contatto blocchi difettoso
2. ingresso scheda difettoso (pin 6-7, vedi [layout](../../layouts/mcpx.md))
3. cavo di vano difettoso

#### Soluzioni
1. controllare contatto blocchi
2. mandare scheda in assistenza
3. controllare cavo di vano

---

## Codice 023 {#023}
Teleruttore SAL non attratto in salita.

#### Descrizione
È stata fatta una partenza in salita e il teleruttore SAL non si è attratto.

#### Cause
1. teleruttore difettoso
2. tensione di manovra bassa
3. uscita scheda difettosa (pin 68, vedi [layout](../../layouts/mcpx.md))
4. ingresso di feedback della scheda difettoso (pin 39, vedi [layout](../../layouts/mcpx.md))
5. contatto di feedback del teleruttore alla scheda difettoso

#### Soluzioni
1. cambiare teleruttore
2. controllare tensione di manovra ad inizio e fine serie durante il funzionamento e identificare il circuito che provoca il calo di tensione
3. 4 mandare scheda in assistenza
5. cabiare contatto o teleruttore

---

## Codice 024 {#024}
Il contatto 8-9 (morsetti del quadro) delle serie di sicurezza si è aperto mentre la cabina viaggiava in salita.

#### Cause
1. contatto porte cabina difettoso
2. ingresso scheda difettoso (pin 5-6, vedi [layout](../../layouts/mcpx.md))
3. cavo di vano difettoso

#### Soluzioni
1. controllare contatto porte cabina
2. mandare scheda in assistenza
3. controllare cavo di vano

---

## Codice 025 {#025}
Teleruttore DIS attratto in salita.

#### Descrizione
È stata effettuata una partenza in salita e il teleruttore DIS è rimasto attratto.

#### Cause
1. teleruttore difettoso
2. contatto di feedback del teleruttore alla scheda difettoso
3. ingresso di feedback della scheda difettoso (pin 49, vedi [layout](../../layouts/mcpx.md)))
4. uscita di comando della scheda difettosa (pin 67, vedi [layout](../../layouts/mcpx.md)))

#### Soluzioni
1. cambiare teleruttore
2. cabiare contatto o teleruttore
3. 4 mandare scheda in assistenza

---

## Codice 026 {#026}
Contatti pre-finecorsa aperti in alta velocità (impianto a fune con VVVF).

#### Descrizione
In impianti veloci per ragioni di sicurezza vengono usati 2 contatti aggiuntivi oltre al finecorsa di salita e di discesa.
Questi contatti (prefinecorsa) sono meccanici e devono aprirsi dopo che si è aperto il rispettivo finecorsa e prima della fermata.

#### Cause
1. contatto difettoso
2. cavo di vano difettoso
3. ingresso scheda difettoso (pin 80 e 83, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. sostituire contatto
2. controllare cavo di vano
3. mandare scheda in assistenza

---

## Codice 027 {#027}
Contatto blocchi aperto in alta velocità (impianto a fune con VVVF).

#### Descrizione
Il contatto 9-10 (morsetti del quadro) delle serie di sicurezza si è aperto mentre la cabina viaggiava in alta velocità. Questo errore viene segnalato solo in impianti a fune con VVVF.

#### Cause
1. contatto blocchi difettoso
2. ingresso scheda difettoso (pin 6-7, vedi [layout](../../layouts/mcpx.md))
3. cavo di vano difettoso

#### Soluzioni
1. controllare contatto blocchi
2. mandare scheda in assistenza
3. controllare cavo di vano

---

## Codice 028 {#028}
Teleruttore P non attratto.

#### Descrizione
È stata effettuata una partenza e il teleruttore P non si è attratto.

#### Cause
1. teleruttore difettoso
2. tensione di manovra bassa
3. uscita scheda difettosa (pin 65, vedi [layout](../../layouts/mcpx.md))
4. ingresso di feedback della scheda difettoso (pin 41, vedi [layout](../../layouts/mcpx.md))
5. contatto di feedback del teleruttore alla scheda difettoso

#### Soluzioni
1. cambiare teleruttore
2. controllare tensione di manovra ad inizio e fine serie durante il funzionamento e identificare il circuito che provoca il calo di tensione
3. 4 mandare scheda in assistenza
5. cambiare contatto o teleruttore

---

## Codice 029 {#029}
Porte cabina automatiche aperte in alta velocità (impianto a fune con VVVF).

#### Descrizione
Il contatto delle porte cabina (morsetti 8-9 del quadro) della catena delle sicurezze si è aperto mentre l'impianto era in alta velocità.
Questo codice viene segnalato solo in impianti a fune con VVVF.

#### Cause
1. contatto perte cabina difettoso
2. ingresso scheda difettoso (pin 5-6, vedi [layout](../../layouts/mcpx.md))
3. cavo di vano difettoso

#### Soluzioni
1. controllare contatto blocchi
2. mandare scheda in assistenza
3. controllare cavo di vano

---

## Codice 030 {#030}
Mancata risposta del VVVF in bassa al cambio di velocità.

#### Descrizione
Il VVVF non ha attivato la propria uscita al cambio di velocità. L'uscita del VVVF può essere configurata per dare un segnale
al cambio di velocità. Questo segnale viene letto sul pin 44 della scheda (vedi [layout](../../layouts/mcpx.md)).
Questo ingresso può essere impostato con il parametro [025](../parametri/manovra.md#025).

#### Cause
#### Soluzioni

---

## Codice 031 {#031}
Contatti prefinecorsa aperti in bassa velocità (impianto a fune con VVVF).

#### Descrizione
Questo errore si verifica in due casi:
1. al cambio di velocità ai piani intermedi si sono aperti i prefinecorsa di salita/discesa
   (secondo la direzione della cabina)
2. ai piani estremi all'apertura del prefinecorsa non è intervenuto il contatto di bypass del VVVF

#### Cause
1. contatto VVVF difettoso
2. cavo di vano difettoso
3. ingresso scheda difettoso (pin 80 e 83, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. sostituire contatto VVVF
2. controllare cavo di vano
3. mandare scheda in assistenza

---

## Codice 032 {#032}
Contatto blocchi aperto in bassa velocità (impianto a fune con VVVF).

#### Descrizione
Il contatto 9-10 (morsetti del quadro) delle serie di sicurezza si è aperto mentre la cabina viaggiava in bassa velocità. Questo errore viene segnalato solo in impianti a fune con VVVF.

#### Cause
1. contatto blocchi difettoso
2. ingresso scheda difettoso (pin 6-7, vedi [layout](../../layouts/mcpx.md))
3. cavo di vano difettoso

#### Soluzioni
1. controllare contatto blocchi
2. mandare scheda in assistenza
3. controllare cavo di vano

---

## Codice 033 {#033}
Teleruttori di marcia TM-TM1 non attratti in bassa velocità (impianto a fune con VVVF).

#### Descrizione
È stato effettuato il passaggio da alta velocità a bassa velocità e i teleruttori TM-TM1 non erano attratti.

#### Cause
1. teleruttori difettosi
2. contatti di feedback dei teleruttori alla scheda difettosi (vedi schema)
3. ingresso di feedback della scheda difettoso (pin 41, vedi [layout](../../layouts/mcpx.md))
4. comando scheda difettoso (pin 71, vedi [layout](../../layouts/mcpx.md))
5. bassa tensione di manovra


#### Soluzioni
1. cambiare teleruttori
2. cambiare contatti o teleruttori
3. 4 mandare scheda in assistenza
5. controllare tensione di manovra ad inizio e fine serie durante il funzionamento e identificare il circuito che provoca il calo di tensione

---

## Codice 034 {#034}
Porte cabina automatiche aperte in bassa velocità (impianto a fune con VVVF).
#### Descrizione
Il contatto 8-9 relativo alle porte cabina si è aperto mentre la cabina viaggiava in bassa velocità.

#### Cause
1. contatto porte cabina difettoso
2. ingresso scheda difettoso (pin 5-6, vedi [layout](../../layouts/mcpx.md))
3. cavo di vano difettoso

#### Soluzioni
1. controllare contatto porte cabina
2. mandare scheda in assistenza
3. controllare cavo di vano

---

## Codice 035 {#035}
Mancata risposta del VVVF alla fine della rampa di rallentamento.
#### Descrizione
Alla fermata il VVVF genera un segnale (apre un contatto) per segnalare alla scheda del quadro di avviare la sequenza di fermata.
Questo segnale è mancato e la scheda ha fermato la manovra.

#### Cause
1. contatto VVVF difettoso (vedi schema del quadro)
2. ingresso di feedback della scheda difettoso (pin 44, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. se non è possibile programmare VVVF per usare un'altra uscita, madare VVVF in assistenza
2. mandare scheda in assistenza

---

## Codice 036 {#036}
5 tentativi di rifasamento falliti.
#### Descrizione
All'accensione della scheda la prima cosa che viene effettuata è un rifasamento dell'impianto (ritorno al piano più basso).
La partenza viene provata per 5 volte, dopodichè viene __bloccato l'impianto__.
Controllare gli errori precedenti a questo per risalire alle cause del blocco.

#### Cause
Qualsiasi condizione che possa bloccare la partenza:
* blocchi aperti
* fotocellula interrotta etc...

#### Soluzioni
Controllare che non ci siano condizioni che impediscono la partenza.

---

## Codice 037 {#037}
Fine tempo di tenuta manovra in attesa che il contatto dei blocchi si chiuda.

#### Descrizione
Quando viene dato il comando di partenza, vengono aspettati circa 15 secondi per la chiusura dei blocchi.

#### Cause
1. contatto blocchi difettoso
2. ingresso scheda difettoso (pin 6-7, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. controllare contatto blocchi
2. mandare scheda in assistenza

---

## Codice 038 {#038}
Fine tempo di tenuta manovra in attesa che le porte di cabina automatiche si chiudano.

#### Descrizione
Quando viene dato il comando di partenza, vengono aspettati circa 15 secondi per la chiusura del contatto di porte cabina.

#### Cause
1. contatto porte cabina difettoso
2. ingresso scheda difettoso (pin 5-6, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. controllare contatto blocchi
2. mandare scheda in assistenza

---

## Codice 039 {#039}
Fine tempo di tenuta manovra in attesa che i contatti dei pre-finecorsa si chiudano.
#### Descrizione
In impianti veloci per ragioni di sicurezza vengono usati 2 contatti aggiuntivi oltre al finecorsa di salita e di discesa.
Questi contatti (prefinecorsa) sono meccanici e devono aprirsi dopo che si è aperto il rispettivo finecorsa e prima della fermata.

#### Cause
1. contatto difettoso
2. cavo di vano difettoso
3. ingresso scheda difettoso (pin 80 e 83, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. sostituire contatto
2. controllare cavo di vano
3. mandare scheda in assistenza

---

## Codice 040 {#040}
Fine tempo di tenuta manovra in attesa che il teleruttore P si attragga con catena contatti sicurezze chiusa.

#### Descrizione
È stato dato il comando di marcia ma il teleruttore P non si è attratto.

#### Cause
1. teleruttore difettoso
2. contatto di feedback del teleruttore alla scheda difettoso (vedi shcema quadro)
3. ingresso di feedback della scheda difettoso (pin 41, vedi [layout](../../layouts/mcpx.md))
4. uscita di comando della scheda difettosa (pin 65, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. cambiare teleruttore
2. cambiare contatto o teleruttore
3. 4 mandare scheda in assistenza

---

## Codice 041 {#041}
Fine tempo di tenuta manovra in attesa che il teleruttore SAL si attragga con catena contatti sicurezze chiusa.

#### Descrizione
È stato dato il comando di marcia in salita ma il teleruttore SAL non si è attratto.

#### Cause
1. teleruttore difettoso
2. contatto di feedback del teleruttore alla scheda difettoso (vedi shcema quadro)
3. ingresso di feedback della scheda difettoso (pin 39, vedi [layout](../../layouts/mcpx.md))
4. uscita di comando della scheda difettosa (pin 68, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. cambiare teleruttore
2. cambiare contatto o teleruttore
3. 4 mandare scheda in assistenza

---

## Codice 042 {#042}
Fine tempo di tenuta manovra in attesa che il teleruttore DIS si attragga con catena contatti sicurezze chiusa.

#### Descrizione
È stato dato il comando di marcia in dicsesa ma il teleruttore DIS non si è attratto.

#### Cause
1. teleruttore difettoso
2. contatto di feedback del teleruttore alla scheda difettoso (vedi shcema quadro)
3. ingresso di feedback della scheda difettoso (pin 40, vedi [layout](../../layouts/mcpx.md))
4. uscita di comando della scheda difettosa (pin 67, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. cambiare teleruttore
2. cambiare contatto o teleruttore
3. 4 mandare scheda in assistenza

---

## Codice 043 {#043}
Relè PV non attratto alla partenza (impianto oleodinamico).

#### Descrizione
È stato dato il comando di marcia in alta velocità per partire ma PV non si è attratto.

#### Cause
1. relè difettoso
2. contatto di feedback del relè alla scheda difettoso (vedi schema del quadro)
3. ingresso di feedback della scheda difettoso (pin 42, vedi [layout](../../layouts/mcpx.md))
4. uscita di comando della scheda difettoso (pin 66, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. 2 cambiare relè
3. 4 mandare scheda in assistenza

---

## Codice 044 {#044}
Teleruttore Y non attratto alla partenza (impianto oleodinamico con avviamento stella-triangolo).

#### Descrizione
È stato dato il comando di marcia in salita ma il teleruttore Y non si è attratto.

#### Cause
1. teleruttore difettoso
2. interblocco tra teleruttore SAL e Y difettoso
3. contatto di feedback del teleruttore alla scheda difettoso (vedi scheda del quadro)
4. ingresso di feedback della scheda difettoso (pin 39, vedi [layout](../../layouts/mcpx.md))
5. uscita di comando della scheda difettosa (pin 71, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. cambiare teleruttore
2. cambiare interblocco
3. cambiare contatto o teleruttore
4. 5 mandare scheda in assistenza

---

## Codice 045 {#045}
Teleruttore Y non attratto all'avvio del ripescamento in salita (impianto oleodinamico con avviamento stella-triangolo).

#### Descrizione
È stato provato un ripescaggio in salita ma il teleruttore Y non si è attratto.

#### Cause
1. teleruttore difettoso
2. interblocco tra teleruttore SAL e Y difettoso
3. contatto di feedback del teleruttore alla scheda difettoso (vedi scheda del quadro)
4. ingresso di feedback della scheda difettoso (pin 39, vedi [layout](../../layouts/mcpx.md))
5. uscita di comando della scheda difettosa (pin 71, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. cambiare teleruttore
2. cambiare interblocco
3. cambiare contatto o teleruttore
4. 5 mandare scheda in assistenza

---

## Codice 046 {#046}
Teleruttore SAL non attratto all'avvio del ripescamento in salita (impianto oleodinamico).

#### Descrizione
È stato provato un ripescaggio in salita ma il teleruttore SAL non si è attratto.

#### Cause
1. teleruttore difettoso
2. interblocco tra teleruttore SAL e Y difettoso (se avviamento stella triangolo)
3. contatto di feedback del teleruttore alla scheda difettoso (vedi scheda del quadro)
4. ingresso di feedback della scheda difettoso (pin 39, vedi [layout](../../layouts/mcpx.md))
5. uscita di comando della scheda difettosa (pin 68, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. cambiare teleruttore
2. cambiare interblocco
3. cambiare contatto o teleruttore
4. 5 mandare scheda in assistenza

---

## Codice 047 {#047}
Teleruttore P non attratto all'avvio del ripescamento in salita (impianto oleodinamico).

#### Descrizione
È stato provato un ripescaggio in salita ma il teleruttore P non si è attratto.

#### Cause
1. teleruttore difettoso
2. contatto di feedback del teleruttore alla scheda difettoso (vedi schema del quadro)
3. ingresso di feedback della scheda difettoso (pin 41, vedi [layout](../../layouts/mcpx.md))
4. uscita di comando della scheda difettosa (pin 65, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. cambiare teleruttore
2. cambiare contatto o teleruttore
3. 4 mandare scheda in assistenza

---

## Codice 048 {#048}
Relè PV attratto all'avvio del ripescamento in salita (impianto oleodinamico).

#### Descrizione
È stato avviato un ripescaggio in salita e il relè PV è rimasto attratto.

#### Cause
1. relè difettoso
#### Soluzioni

---

## Codice 049 {#049}
Teleruttori P e SAL non attratti all'avvio del ripescamento in salita (impianto oleodinamico con avviamento diretto o soft-starter).

#### Descrizione
È stato dato il comando di ripescamento in salita ma i teleruttori P e SAL non si sono attratti.

#### Cause
1. teleruttori difettosi
2. contatti di feedback dei teleruttori alla scheda difettosi (vedi lo schema del quadro)
3. ingressi di feedback della scheda difettosi (pin 41 e 39, vedi [layout](../../layouts/mcpx.md))
4. uscite di comando della scheda difettose (pin 65 e 68, vedi [layout](../../layouts/mcpx.md))
5. tensione di manvora bassa

#### Soluzioni
1. cambiare teleruttori
2. cambiare contatti o teleruttori
3. 4 mandare scheda in assistenza
5. controllare tensione di manovra ad inizio e fine serie durante il funzionamento e identificare il circuito che provoca il calo di tensione

---

## Codice 050 {#050}
Teleruttore P non attratto all'avvio del ripescamento in salita (impianto oleodinamico).

#### Descrizione
È stato dato il comando di ripescamento in salita ma il teleruttore P non si è attratto.

#### Cause
1. teleruttore difettoso
2. contatto di feedback del teleruttore alla sceda difettoso (vedi schema quadro)
3. ingresso di feedback della scheda difettoso (pin 41, vedi [layout](../../layouts/mcpx.md))
4. uscita di comando della scheda difettosa (pin 65, vedi [layout](../../layouts/mcpx.md))
5. bassa tensione di manovra

#### Soluzioni
1. cambiare teleruttori
2. cambiare contatti o teleruttori
3. 4 mandare scheda in assistenza
5. controllare tensione di manovra ad inizio e fine serie durante il funzionamento e identificare il circuito che provoca il calo di tensione

---

## Codice 051 {#051}
Modulo sicurezza RSS non attratto dopo avvio ripescamento in salita (impianto oleodinamico).

#### Descrizione
È stato dato il comando di ripescaggio in salita ma l'uscita di abilitazione del modulo RSS non era attiva.

#### Cause
1. modulo difettoso
2. ingresso di feedback della scheda difettoso (pin 44, vedi [layout](../../layouts/mcpx.md))
3. ingressi della scheda di lettura zona di controllo ripecaggio difettosi (pin 19 e 21, vedi [layout](../../layouts/mcpx.md))
4. uscite della scheda per comando ingressi RSS difettose (pin 22-23, 15-16, vedi [layout](../../layouts/mcpx.md))
5. accoppiamento pista e induttore IZ1-IZ2 errato
6. cavo di cabina difettoso

#### Soluzioni
1. cambiare modulo
2. 3, 4 mandare scheda in assistenza
5. assicurarsi che lo spazio tra l'induttore e la pista non sia maggiore di 1cm.
6. cantrolla re cavo cabina

---

## Codice 052 {#052}
Induttore ID aperto nel ripescamento in salita (impianto oleodinamico).

#### Descrizione
Durante il ripecaggio in salita si è aperto l'induttore ID.

#### Cause
1. induttore difettoso
2. interferenze magnetiche
3. cavo di cabina difettoso
4. accoppiamento pista magnetica e induttore non corretto
5. piste di fermata registrate non correttamente

#### Soluzioni
1. cambiare induttore
2. posizionare le piste di fermata con lati opposti (ad esempio una con lato gialla ed una con lato nero)
3. controllare cavo di cabina
4. controllare che la distanza tra induttore e pista non sia maggiore di 1cm
5. assicurarsi che lo spazio di sovrapposizione tra le piste di fermata sia di almeno 2cm, regolare la fermata con i parametri [015](../parametri/temporizzazioni.md#015) e [016](../parametri/temporizzazioni.md#016)

---

## Codice 053 {#053}
Teleruttore SAL non attratto all'avvio del ripescamento in salita (impianto oleodinamico).

#### Descrizione
È stato dato il comando di ripecaggio in salita ma il teleruttore SAL non si è attratto.

#### Cause
1. teleruttore difettoso
2. tensione di manovra bassa
3. uscita scheda difettosa (pin 68, vedi [layout](../../layouts/mcpx.md))
4. ingresso di feedback della scheda difettoso (pin 39, vedi [layout](../../layouts/mcpx.md))
5. contatto di feedback del teleruttore alla scheda difettoso

#### Soluzioni
1. cambiare teleruttore
2. controllare tensione di manovra ad inizio e fine serie durante il funzionamento e identificare il circuito che provoca il calo di tensione
3. 4 mandare scheda in assistenza
5. cabiare contatto o teleruttore

---

## Codice 054 {#054}
Teleruttore P non attratto all'avvio del ripescamento in salita (impianto oleodinamico).

#### Descrizione
È stato dato il comando di ripescaggio in salita ma il teleruttore P non si è attratto.

#### Cause
1. teleruttore difettoso
2. tensione di manovra bassa
3. uscita scheda difettosa (pin 65, vedi [layout](../../layouts/mcpx.md))
4. ingresso di feedback della scheda difettoso (pin 41, vedi [layout](../../layouts/mcpx.md))
5. contatto di feedback del teleruttore alla scheda difettoso

#### Soluzioni
1. cambiare teleruttore
2. controllare tensione di manovra ad inizio e fine serie durante il funzionamento e identificare il circuito che provoca il calo di tensione
3. 4 mandare scheda in assistenza
5. cambiare contatto o teleruttore

---

## Codice 055 {#055}
Relè PV attratto nel ripescamento in discesa (impianto oleodinamico).

#### Descrizione
È stato dato il comando di ripescaggio e il relè PV è rimasto attratto.

#### Cause
1. relè difettoso
2. contatto relè di feedback alla scheda difettoso (vedi schema del quadro)
3. ingresso feedback della scheda difettoso (pin 42, vedi [layout](../../layouts/mcpx.md))
4. uscita di comando scheda difettosa (pin 66, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. cambiare il relè
2. cambiare relè
3. 4 mandare scheda in assistenza

---

## Codice 056 {#056}
Teleruttore P e relè DIS non attratti all'avvio del ripescamento in discesa (impianto oleodinamico).

#### Descrizione
È stato dato il comando di ripescaggio in discesa ma il teleruttore P e il relè DIS non si sono attratti.

#### Cause
1. teleruttore e relè difettosi
2. tensione di manovra bassa
3. uscita scheda difettosa (pin 67, vedi [layout](../../layouts/mcpx.md))
4. ingresso di feedback della scheda difettoso (pin 40, vedi [layout](../../layouts/mcpx.md))
5. contatto di feedback del teleruttore e relè alla scheda difettoso (vedi schema del quadro)

#### Soluzioni
1. cambiare teleruttore e/o relè
2. controllare tensione di manovra ad inizio e fine serie durante il funzionamento e identificare il circuito che provoca il calo di tensione
3. 4 mandare scheda in assistenza
5. cambiare contatto o teleruttore e relè

---

## Codice 057 {#057}
Modulo sicurezza non attratto dopo avvio ripescamento in discesa (impianto oleodinamico).

#### Descrizione
È stato dato il comando di ripescaggio in salita ma l'uscita di abilitazione del modulo RSS non era attiva.

#### Cause
1. modulo difettoso
2. ingresso di feedback della scheda difettoso (pin 44, vedi [layout](../../layouts/mcpx.md))
3. ingressi della scheda di lettura zona di controllo ripecaggio difettosi (pin 19 e 21, vedi [layout](../../layouts/mcpx.md))
4. uscite della scheda per comando ingressi RSS difettose (pin 22-23, 15-16, vedi [layout](../../layouts/mcpx.md))
5. accoppiamento pista e induttore IZ1-IZ2 errato
6. cavo di cabina difettoso

#### Soluzioni
1. cambiare modulo
2. 3, 4 mandare scheda in assistenza
5. assicurarsi che lo spazio tra l'induttore e la pista non sia maggiore di 1cm.
6. cantrolla re cavo cabina

---

## Codice 058 {#058}
Induttore IS aperto nel ripescamento in discesa (impianto oleodinamico).

#### Descrizione
Durante il ripecaggio in discesa si è aperto l'induttore IS.

#### Cause
1. induttore difettoso
2. interferenze magnetiche
3. cavo di vano difettoso
4. accoppiamento pista magnetica e induttore non corretto
5. piste di fermata registrate non correttamente

#### Soluzioni
1. cambiare induttore
2. posizionare le piste di fermata con lati opposti (ad esempio una con lato gialla ed una con lato nero)
3. controllare cavo di vano
4. controllare che la distanza tra induttore e pista non sia maggiore di 1cm
5. assicurarsi che lo spazio di sovrapposizione tra le piste di fermata sia di almeno 2cm, regolare la fermata con i parametri [015](../parametri/temporizzazioni.md#015) e [016](../parametri/temporizzazioni.md#016)

---

## Codice 059 {#059}
Relè DIS non attratto all'avvio del ripescamento in discesa (impianto oleodinamico).

#### Descrizione
È stato dato il comando di ripecaggio in discesa ma il teleruttore DIS non si è attratto.

#### Cause
1. teleruttore difettoso
2. tensione di manovra bassa
3. uscita scheda difettosa (pin 67, vedi [layout](../../layouts/mcpx.md))
4. ingresso di feedback della scheda difettoso (pin 40, vedi [layout](../../layouts/mcpx.md))
5. contatto di feedback del teleruttore alla scheda difettoso

#### Soluzioni
1. cambiare teleruttore
2. controllare tensione di manovra ad inizio e fine serie durante il funzionamento e identificare il circuito che provoca il calo di tensione
3. 4 mandare scheda in assistenza
5. cabiare contatto o teleruttore

---

## Codice 060 {#060}
Relè DIS attratto nel ripescamento in salita (impianto oleodinamico).

#### Descrizione
È stato dato il comando di ripescaggio in salita e il relè DIS è rimasto attratto.

#### Cause
1. teleruttore difettoso
2. contatto di feedback del teleruttore alla scheda difettoso
3. ingresso di feedback della scheda difettoso (pin 49, vedi [layout](../../layouts/mcpx.md)))
4. uscita di comando della scheda difettosa (pin 67, vedi [layout](../../layouts/mcpx.md)))

#### Soluzioni
1. cambiare teleruttore
2. cabiare contatto o teleruttore
3. 4 mandare scheda in assistenza

---

## Codice 061 {#061}
Teleruttore SAL attratto nel ripescamento in discesa (impianto oleodinamico).
#### Descrizione
È stato dato il comando di ripescaggio in discesa e il teleruttore di salita è rimasto attratto.

#### Cause
1. teleruttore difettoso
2. contatto di feedback del teleruttore alla scheda difettoso (vedi schema quadro)
3. ingresso di feedback della scheda difettoso (pin 39, vedi [layout](../../layouts/mcpx.md)))
4. uscita di comando della scheda difettosa (pin 68, vedi [layout](../../layouts/mcpx.md)))

#### Soluzioni
1. cambiare teleruttore
2. cabiare contatto o teleruttore
3. 4 mandare scheda in assistenza

---

## Codice 062 {#062}
Scaduto tempo ripescamento in salita (impianto oleodinamico).

#### Descrizione
Il comando di ripescaggio in salita è rimasto attivo per troppo tempo senza che la cabina sia ritornata al piano.

#### Cause
Relè e/o teleruttori (SAL, P, Y) di marcia difettosi.

#### Soluzioni
Cambiare relè e/o teleruttori di marcia.

---

## Codice 063 {#063}
Scaduto tempo ripescamento in discesa (impianto oleodinamico).

#### Descrizione
Il comando di ripescaggio in discesa è rimasto attivo per troppo tempo senza che la cabina sia ritornata al piano.

#### Cause
Relè e/o teleruttori (P, DIS) di marcia difettosi.

#### Soluzioni
Cambiare relè e/o teleruttori di marcia.

---

## Codice 064 {#064}
Scaduto tempo corsa.

#### Descrizione
L'impianto è rimasto in movimento senza avere nessun feedback dai finecorsa (FCS,FCD) per un tempo superiore a quello impostato nel parametro [000](../parametri/temporizzazioni.md#000).

#### Cause
1. bistabili difettosi
2. accoppiamento pista magnetica e induttore/bistabile non corretto
3. cavo di cabina difettoso
4. ingressi scheda difettosi (pin 55-56-57-58, vedi [layout](../../layouts/mcpx.md))
5. relè e/o (SAL, P, PV, DIS, Y) teleruttori di marcia difettosi

#### Soluzioni
1. cambiare induttori e bistabili
2. controllare che la distanza tra induttori e bistabili con piste non sia maggiore di 1cm
3. controllare cavo di cabina
4. mandare scheda in assistenza
5. cambiare relè e/o teleruttori di marcia

---

## Codice 065 {#065}
Scaduto tempo bassa velocità.

#### Descrizione
La cabina è rimasta in movimento in bassa velocità senza avere un feedback dagli induttori IS e ID per un tempo superiore a
quello impostato nel parametro [014](../parametri/temporizzazioni.md#014).

#### Cause
1. interferenza magnetiche
2. accoppiamento piste magnetiche e induttori non corretto
3. cavo di cabina difettoso
4. relè e o teleruttori di comando bassa velocità difettosi (PV, SAL, DIS)
5. induttori difettosi
6. VVVF non tarato correttamente

#### Soluzioni
1. posizionare le piste di fermata con lati opposti (ad esempio una con lato gialla ed una con lato nero)
2. controllare che la distanza tra induttore e pista non sia maggiore di 1cm
3. controllare cavo di cabina
4. cambiare relè e/o teleruttori di comando di bassa velocità
5. cambiare induttori
6. effettuare taratura VVVF

---

## Codice 066 {#066}
Ripristino conteggio discesa dal conteggio di salita.

#### Descrizione
Durante ogni viaggio vengono contate separatemente le piste di discesa e di salita incontrate nella corsa. Per andare dal piano A al piano B sono presenti nel vano N piste di salita e N piste di discesa.
Alla fermata (induttori IS e ID  chiusi) viene confrontato il numero di piste di salita e discesa contate con il numero N.
In questo caso il numero di piste di discesa contate è diverso da N, mentre quelle di salita è giusto, quindi viene ripristinato il conteggio delle piste di discesa al numero N.

#### Cause
1.   interferenze magnetiche
2.   accoppiamento piste magnetiche e induttori non corretto
3.   induttori difettosi
4.   cavo di cabina difettoso
5. piste di fermata registrate non correttamente

#### Soluzioni
1.   posizionare le piste di fermata con lati opposti (ad esempio una con lato gialla ed una con lato nero)
2.   controllare che la distanza tra induttori e piste non sia maggiore di 1cm
3.   controllare che gli induttori non siano difettosi
4.   controllare che il cavo di cabina non sia interrotto
5. assicurarsi che lo spazio di sovrapposizione tra le piste di fermata sia di almeno 2cm, regolare la fermata con i parametri [015](../parametri/temporizzazioni.md#015) e [016](../parametri/temporizzazioni.md#016)

---

## Codice 067 {#067}
Ripristino conteggio salita dal conteggio di discesa.

#### Descrizione
Durante ogni viaggio vengono contate separatemente le piste di discesa e di salita incontrate nella corsa. Per andare dal piano A al piano B sono presenti nel vano N piste di salita e N piste di discesa.
Alla fermata (induttori IS e ID  chiusi) viene confrontato il numero di piste di salita e discesa contate con il numero N.
In questo caso il numero di piste di salita contate è diverso da N, mentre quelle di discesa è giusto, quindi viene ripristinato il conteggio delle piste di salita al numero N.

#### Cause
1.   interferenze magnetiche
2.   accoppiamento piste magnetiche e induttori non corretto
3.   induttori difettosi
4.   cavo di cabina difettoso
5.   piste di fermata registrate non correttamente

#### Soluzioni
1.   posizionare le piste di fermata con lati opposti (ad esempio una con lato giall ed una con lato nero)
2.   controllare che la distanza tra induttori e piste non sia maggiore di 1cm
3.   controllare che gli induttori non siano difettosi
4.   controllare che il cavo di cabina non sia interrotto
5.  assicurarsi che lo spazio di sovrapposizione tra le piste di fermata sia di almeno 2cm, regolare la fermata con i parametri [015](../parametri/temporizzazioni.md#015) e [016](../parametri/temporizzazioni.md#016)

---

## Codice 068 {#068}
Effettuata una chiamata ad un piano più alto del numero di fermate.

#### Descrizione

Non si può effettuare una chiamata ad un piano che in teoria non esiste.

#### Cause
Errata programmazione scheda madre e/o periferiche.

#### Soluzioni
Assicurarsi di aver programmato un numero di fermate (parametro [046](../parametri/manovra.md#046)) che sia in accordo
con gli indirizzi programmati nelle periferiche del quadro (vedi [elenco indirizzi periferiche](../../../periferiche/indirizzi.md)).

---

## Codice 069 {#069}
Entrambi i finecorsa (FCS e FCD) sono aperti, non è possibile effettuare partenza.

#### Descrizione
La situazione in cui entrambi i finecorsa sono aperti è considerata una ragione sufficiente per non effettuare la partenza.

#### Cause
1. bistabili difettosi
2. accoppiamento bistabili e piste magnetiche non corretto
3. cavo di cabina difettoso
4. ingressi della scheda difettosi (pin 57-58, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. cambiare bistabili
2. assicurarsi che la distanza tra bistabile e pista sia meno di 1cm e che il versio della pista sia quello giusto
3. controllare cavo di cabina
4. mandare scheda in assistenza

---

## Codice 070 {#070}
Induttore IS aperto alla fermata per scivolamento.

#### Descrizione
Dopo il comando di fermata (induttori IS e ID chiusi) viene avviato un timer dalla durata fissa di 4 secondi.
Se in questo frangente l'induttore IS si apre viene dedotto che l'impianto ha scivolato.

#### Cause

#### Soluzioni

---

## Codice 071 {#071}
Induttore ID aperto alla fermata per scivolamento.

#### Descrizione
Dopo il comando di fermata (induttori IS e ID chiusi) viene avviato un timer dalla durata fissa di 4 secondi.
Se in questo frangente l'induttore ID si apre viene dedotto che l'impianto ha scivolato.

#### Cause

#### Soluzioni

---

## Codice 072 {#072}
Induttore ID aperto con impianto fermo per deriva dovuta ad elasticità funi o manovra a mano.

#### Descrizione
Dopo il comando di fermata (induttori IS e ID chiusi), scaduto il timer di 4 secondi di controllo
di scivolamento della cabina ([vedi errore 070 o 071](#070)), si è aperto l'induttore ID.
Viene dedotto che le funi hanno troppa elasticità o la cabina è stata spostata a mano.
Questo errore è __escluso__ nell'__impianto oleodinamico__.

#### Cause

#### Soluzioni

---

## Codice 073 {#073}
Induttore IS aperto con impianto fermo per deriva dovuta ad elasticità funi o manovra a mano.

#### Descrizione
Dopo il comando di fermata (induttori IS e ID chiusi), scaduto il timer di 4 secondi di controllo
di scivolamento della cabina ([vedi errore 070 o 071](#070)), si è aperto l'induttore IS.
Viene dedotto che le funi hanno troppa elasticità o la cabina è stata spostata a mano.
Questo errore è __escluso__ nell'__impianto oleodinamico__.

#### Cause

#### Soluzioni

---

## Codice 075 {#075}
Il contatto di controllo del relè AP è rimasto chiuso per oltre 25 secondi.

#### Descrizione
Il relè AP ha un contatto che viene usato come feedback dalla scheda per sapere se è attratto o meno. Consultare lo schema specifico del quadro per vedere quale contatto è usato.

#### Cause
1. contatto o relè difettoso
2. interblocco meccanico tra AP e CP difettoso
3. ingresso di feedback della scheda difettoso (pin 31, vedi [layout](../../layouts/mcpx.md))
4. uscita di comando della scheda difettosa (pin 10 o 11, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. cambiare relè
2. cambiare interblocco
3. 4 mandare scheda in assistenza

---

## Codice 076 {#076}
Il contatto di controllo del teleruttore o relè DIS è rimasto chiuso per oltre 25 secondi.

#### Descrizione
Il teleruttore o relè DIS ha un contatto che viene usato come feedback dalla scheda per sapere se è attratto o meno. Consultare lo schema specifico del quadro per vedere quale contatto è usato.

#### Cause
1. contatto o relè difettoso
2. interblocco meccanico tra SAL e DIS difettoso
3. ingresso di feedback della scheda difettoso (pin 40, vedi [layout](../../layouts/mcpx.md))
4. uscita di comando della scheda difettosa (pin 67, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. cambiare relè o teleruttore o contatto
2. cambiare interblocco
3. 4 mandare scheda in assistenza

---

## Codice 077 {#077}
Il contatto di controllo del teleruttore SAL è rimasto chiuso per oltre 25 secondi.

#### Descrizione
Il teleruttore SAL ha un contatto che viene usato come feedback dalla scheda per sapere se è attratto o meno. Consultare lo schema specifico del quadro per vedere quale contatto è usato.

#### Cause
1. contatto o teleruttore difettoso
2. interblocco meccanico tra SAL e DIS difettoso
3. ingresso di feedback della scheda difettoso (pin 39, vedi [layout](../../layouts/mcpx.md))
4. uscita di comando della scheda difettosa (pin 68, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. cambiare teleruttore o contatto
2. cambiare interblocco
3. 4 mandare scheda in assistenza

---

## Codice 078 {#078}
Il contatto di controllo del teleruttore P è rimasto chiuso per oltre 25 secondi.

#### Descrizione
Il teleruttore P ha un contatto che viene usato come feedback dalla scheda per sapere se è attratto o meno. Consultare lo schema specifico del quadro per vedere quale contatto è usato.

#### Cause
1. contatto o teleruttore difettoso
2. ingresso di feedback della scheda difettoso (pin 41, vedi [layout](../../layouts/mcpx.md))
3. uscita di comando della scheda difettosa (pin 65, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. cambiare teleruttore o contatto
2. 3 mandare scheda in assistenza

---

## Codice 079 {#079}
Il contatto di controllo del teleruttore PV è rimasto chiuso per oltre 25 secondi.

#### Descrizione
Il teleruttore o relè PV ha un contatto che viene usato come feedback dalla scheda per sapere se è attratto o meno. Consultare lo schema specifico del quadro per vedere quale contatto è usato.

#### Cause
1. contatto relè o teleruttore difettoso
2. ingresso di feedback della scheda difettoso (pin 41, vedi [layout](../../layouts/mcpx.md))
3. uscita di comando della scheda difettosa (pin 65, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. cambiare relè, teleruttore o contatto
2. 3 mandare scheda in assistenza

---

## Codice 080 {#080}
Nel ripescamento, è scaduto timer di 10 secondi che controlla lo stato del teleruttore P e del
teleruttore Y (impianto oleodinamico con avviamento stella triangolo).

#### Descrizione
Nel ripescaggio viene controllato lo stato del teleruttore P e del teleruttore Y (se sono attratti o meno tramite contatti di feedback in scheda).
In mancanza di feedback il comando viene ripetuto per 10 secondi, dopodichè il ripescaggio viene annullato e segnalato l'errore.
Controllare gli errori precedenti a questo nello storico per risalire alla causa del mancato ripescaggio.

#### Cause
1. teleruttori difettosi
2. contatto di feedback del teleruttore alla scheda difettoso (vedi schema del quadro)
3. ingressi di feedback della scheda difettoso (vedi [layout](../../layouts/mcpx.md))
4. uscite di comando della scheda difettose (vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. cambiare teleruttore/i
2. cambiare contatto/i di feedback
3. 4. mandare scheda in assistenza

---

## Codice 081 {#081}
Relè RSS o relè RRSS non hanno fatto bypass dei contatti delle sicurezze nella zona di sicurezza di piano.

#### Descrizione
In impianti oleodinamici, nella zona di sicurezza di piano il relè RSS del quadro e il relè RRSS della scheda (vedi [layout](../../layouts/mcpx.md))
bypassano i contatti delle porte per permettere il ripescaggio dell'impianto con porte aperte. La scheda controlla per
10 secondi lo stato dei teleruttori di marcia e, se questi non sono attratti, ne deduce che il bypass non è avvenuto.

#### Cause
1. relè RSS difettoso
2. relè RRSS difettoso (vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. sostituire relè
2. mandare scheda in assistenza

---

## Codice 082 {#082}
Mancata risposta del VVVF all'avvio o in marcia.

#### Descrizione
Quando viene dato il comando di marcia al VVVF questo chiude un contatto N.O. (contatto OUT) per segnalare che
ha accettato la richiesta e la marcia è partita. Questo contatto viene letto tramite un ingresso di feedback dalla scheda e, se alla
partenza o in viaggio non è chiuso, viene segnalato questo errore e tolto il comando di marcia.

#### Cause
1. contatto VVVF difettoso (vedi schema del quadro)
2. ingresso di feedback della scheda difettoso (pin 44, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. se non è possibile programmare VVVF per usare un'altra uscita, madare VVVF in assistenza
2. mandare scheda in assistenza

---

## Codice 083 {#083}
Induttori IS e ID chiusi in viaggio all'apertura del finecorsa di discesa FCD.

#### Descrizione
La cabina era in viaggio in discesa, si è aperto FCD ma gli induttori di fermata IS e ID erano già chiusi.

#### Cause
1. induttori difettosi
2. piste di fermata posizionate in maniera errata
3. ingressi della scheda difettosi (pin 55 e 56, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. cambiare induttori
2. assicurarsi che le piste di fermata non siano troop vicine alla pista del finecorsa
3. mandare scheda in assistenza

---

## Codice 084 {#084}
Induttori IS e ID chiusi in viaggio all'apertura del finecorsa di
discesa FCS.

#### Descrizione
La cabina era in viaggio in salita, si è aperto FCS ma gli induttori di fermata IS e ID erano già chiusi.

#### Cause
1. induttori difettosi
2. piste di fermata posizionate in maniera errata
3. ingressi della scheda difettosi (pin 55 e 56, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. cambiare induttori
2. assicurarsi che le piste di fermata non siano troop vicine alla pista del finecorsa
3. mandare scheda in assistenza

---

## Codice 085 {#085}
Esauriti 10 tentativi di partenza con prenotazione.

#### Descrizione
Negli impianti a prenotazione la partenza viene tentata per 10 volte in attesa che eventuali situazioni
che bloccano l'impianto si ripristino (tipo chiusura blocchi, contatto fotocellula / costola mobile etc)

#### Cause
Qualsiasi situazione che può bloccare la partenza dell'impianto:
* blocchi aperti
* fotocellula interrotta
* intervento sovraccarico
* ...

#### Soluzioni
Rimuovere situazione di blocco.

---

## Codice 086 {#086}
Peirferica [41](../../../periferiche/indirizzi.md#indirizzo-41) ferma per 200 millisecondi.

#### Descrizione
Non è stato ricevuto nessun messaggio sul bus seriale dalla periferica [41](../../../periferiche/indirizzi.md#indirizzo-41) per 200 millisecondi. Viene fermato il comando di marcia se attivo.

#### Cause
1. periferica difettosa
2. periferica diconnessa
3. connessione bus difettosa

#### Soluzioni
1. cambiare periferica
2. connettere periferica
3. controllare connessione [bus locale](../../../bus_seriali/README.md#bus-locale)

---

## Codice 087 {#087}
Rimbalzo dei contatti di cabina alla partenza.

#### Descrizione

#### Cause

#### Soluzioni

---

## Codice 088 {#088}
Rimbalzo dei contatti dei blocchi alla partenza.

#### Descrizione

#### Cause

#### Soluzioni

---

## Codice 089 {#089}
Peirferica 41 ferma per 200 millisecondi durante ripescamento (impianto oleodinamico).

#### Descrizione
Non è stato ricevuto nessun messaggio sul bus seriale dalla periferica [41](../../../periferiche/indirizzi.md#indirizzo-41) per 200 millisecondi durante il ripescaggio. Il ripescaggio viene fermato.

#### Cause
1. periferica difettosa
2. periferica diconnessa
3. connessione bus difettosa

#### Soluzioni
1. mandare scheda periferica in assistenza
2. connettere periferica
3. controllare connessione [bus locale](../../../bus_seriali/README.md#bus-locale)

---

## Codice 090 {#090}
Sovraccarico inserito per più di 3 minuti e 20 secondi (impianto a prenotazione).

#### Descrizione
Se l'ingresso del sovraccarico rimane attivo per più di 3 minuti e 20 secondi in impianto a prenotazione viene dedotto che l'impianto
non può camminare e viene attivato il "fuori servizio" e annullate tutte le prenotazioni.

#### Cause
1. impianto in sovraccarico
2. sovraccarico difettoso
3. ingresso della scheda difettoso (pin 51, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. rimuovere causa sovracarico
2. controllare attuatore del sovraccarico
3. mandare scheda in assistenza

---

## Codice 091 {#091}
Ingresso costola mobile dell'ingresso 1 (CM1) inserito per più di 3 minuti e 20 secondi (impianto a prenotazione).

#### Descrizione
Se l'ingresso della contola mobile rimane attivo per più di 3 minuti e 20 secondi in impianto a prenotazione viene dedotto che l'impianto
non può camminare e viene attivato il "fuori servizio" e annullate tutte le prenotazioni.

#### Cause
1. costola mobile o fotocellula interrotta
2. costola mobile o fotocellula difettosa
3. ingresso della scheda difettoso (pin 53, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. rimovere causa dell'interruzione
2. controllare o cambiare costola mobile o fotocellula
3. mandare scheda in assistenza

---

## Codice 092 {#092}
Ingresso costola mobile dell'ingresso 2 (CM2) inserito per più di 3 minuti e 20 secondi (impianto a prenotazione).

#### Descrizione
Se l'ingresso della contola mobile rimane attivo per più di 3 minuti e 20 secondi in impianto a prenotazione viene dedotto che l'impianto
non può camminare e viene attivato il "fuori servizio" e annullate tutte le prenotazioni.

#### Cause
1. costola mobile o fotocellula interrotta
2. costola mobile o fotocellula difettosa
3. ingresso della scheda difettoso (pin 52, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. rimovere causa dell'interruzione
2. controllare o cambiare costola mobile o fotocellula
3. mandare scheda in assistenza

---

## Codice 093 {#093}
Contatto porte cabina in impianti con porte a battente aperto per più di 3 minuti e 20 secondi (impianto a prenotazione).

#### Descrizione
Se il contatto delle porte cabina sulla catenza delle sicurezze (morsetti 8-9 sul quadro) rimane aperto per più di 3 minuti e 20 secondi in impianto a porte a battente e a prenotazione viene dedotto che l'impianto
non può camminare e viene attivato il "fuori servizio" e annullate tutte le prenotazioni.

#### Cause
1. le porte sono state lasciate aperte
2. contatto porte difettoso
3. bassa tensione di manvora
4. ingresso della scheda diffettoso (pin 5-6, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. richuidere le porte
2. controllare contatto porte
3. controllare tensione di manovra ad inizio e fine serie durante il funzionamento e identificare il circuito che provoca il calo di tensione
4. mandare scheda in assistenza

---

## Codice 094 {#094}
Contatto dei preliminari in impianti con porte a battente aperto per più di 3 minuti e 20 secondi (impianto a prenotazione).

#### Descrizione
Se il contatto dei preliminari sulla catenza delle sicurezze (morsetti 7-8 sul quadro) rimane aperto per più di 3 minuti e 20 secondi in impianto a porte a battente e a prenotazione viene dedotto che l'impianto
non può camminare e viene attivato il "fuori servizio" e annullate tutte le prenotazioni.

#### Cause
1. porta di piano lasciata aperta
2. contatto preliminari difettoso
3. bassa tensione di manovra
4. ingresso della scheda difettoso (pin 4-5, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. chiudere porta
2. controllare contatto preliminari
3. controllare tensione di manovra ad inizio e fine serie durante il funzionamento e identificare il circuito che provoca il calo di tensione
4. mandare scheda in assistenza

---

## Codice 095 {#095}
Relè di sicurezza RSS aperto al piano (impianto oleodinamico).

#### Descrizione
Il relè RSS ha aperto il contatto di abilitazione al ripescaggio perchè IZ1-IZ2 si sono aperti al piano.

#### Cause
1. pista di IZ1-IZ2 troppo corta o non centrata
2. accoppiamento IZ1-IZ2 con pista non corretto
3. relè RSS difettoso
4. ingresso della scheda di feedback difettoso (pin 44, vedi [layout](../../layouts/mcpx.md))
5. ingressi IZ1-IZ2 della scheda difettosi (pin 19 e 21, vedi [layout](../../layouts/mcpx.md))
6. uscite IZ1-IZ2 della scheda difettose (pin 15-16 e 22-23, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. assicurarsi che la lunghezza della pista sia giusta (30cm circa) e che sia centrata a livello del piano
2. assicurarsi che la distanza tra IZ1-IZ2 e la pista non sia maggiore di 1cm
3. cambiare relè
4. 5,6 mandare scheda in assistenza

---

## Codice 096 {#096}
Relè di sicurezza RSS rimasto chiuso all'abbandono del piano (impianto oleodinamico).

#### Descrizione
Il contatto di abilitazione del relè di sicurezza RSS è rimasto chiuso quando la cabina ha lasciato il piano in cui si trovava.
La posizione della cabina riportata nell'errore in questo caso è quella del piano successivo o precedente a seconda che questa si
sia mossa in salita o in discesa. Ad esempio, se viene segnalato l'errore al piano 5 e la cabina si è mossa in salita, l'errore si  è verificato
al piano 4.

#### Cause
1. pista di IZ1-IZ2 troppo lunga o non centrata
2. relè RSS difettoso
3. ingresso della scheda di feedback difettoso (pin 44, vedi [layout](../../layouts/mcpx.md))
4. ingressi IZ1-IZ2 della scheda difettosi (pin 19 e 21, vedi [layout](../../layouts/mcpx.md))
5. uscite IZ1-IZ2 della scheda difettose (pin 15-16 e 22-23, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. assicurarsi che la lunghezza della pista sia giusta (30cm circa) e che sia centrata a livello del piano
2. cambiare relè
3. 4,5 mandare scheda in assistenza

---

## Codice 097 {#097}
Nel ripescamento, è scaduto timer di 10 secondi che controlla lo stato dei teleruttori.

#### Descrizione
Nel ripescaggio viene controllato lo stato dei teleruttori di marcia (se sono attratti o meno tramite contatti di feedback in scheda).
In mancanza di feedback il comando viene ripetuto per 10 secondi, dopodichè il ripescaggio viene annullato e segnalato l'errore.
Controllare gli errori precedenti a questo nello storico per risalire alla causa del mancato ripescaggio.

#### Cause
1. teleruttori difettosi
2. contatto di feedback del teleruttore alla scheda difettoso (vedi schema del quadro)
3. ingressi di feedback della scheda difettoso (vedi [layout](../../layouts/mcpx.md))
4. uscite di comando della scheda difettose (vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. cambiare teleruttore/i
2. cambiare contatto/i di feedback
3. 4. mandare scheda in assistenza

---

## Codice 098 {#098}
Il relè AP non si è attratto al comando di apertura porte.

#### Descrizione
Questo errore viene segnalato quando il [parametro 26](../parametri/manovra.md#026) è impostato
con finecorsa apertura porte attivato.

#### Cause
1. relè comando difettoso
2. uscita/e di comando della scheda difettosa (pin 20-10 e 20-11, vedi [layout](../../layouts/mcpx.md))
3. ingresso di feedback della scheda difettoso (pin 37, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. sostituire relè
2. 3. mandare scheda in assistenza
---

## Codice 099 {#099}
Il finecorsa di apertura porte è rimasto chiuso dopo la fine dell'apertura.

#### Descrizione
Questo errore viene segnalato quando il [parametro 26](../parametri/manovra.md#026) è impostato
con finecorsa apertura porte attivato.
Se alla scadenza del tempo impostato nel [parametro 2](../parametri/temporizzazioni.md#002) il relè
di apertura porte è ancora attratto, la scheda deduce che il finecorsa non è intervenuto.

#### Cause
1. finecorsa difettoso
2. relè difettoso
3. contatto di feedback relè difettoso
4. ingresso di feedback della scheda difettoso (pin 37, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. controllare finecorsa
2. sostituire relè
3. sostituire contatto/relè
4. mandare scheda in assistenza

---

## Codice 100 {#100}
Al comandi di apertura porte l'operatore non ha aperto.

#### Descrizione
Se il [parametro 26](../parametri/manovra.md#026) è impostato
con finecorsa apertura porte attivato il relè AP si è attratto ma i contatti delle
porte 8-9 non si sono aperti. La scheda deduce quindi che l'operatore non ha aperto.

Se [parametro 26](../parametri/manovra.md#026) è impostato
con finecorsa apertura porte disattivato il relè AP non è montato e il comando viene dato direttamente
dalla scheda (usato con operatori elettronici).

#### Cause
1. finecorsa difettoso
2. contatti di fase o relè AP difettoso
3. uscita/e di comando della scheda difettosa (pin 20-10 e 20-11, vedi [layout](../../layouts/mcpx.md))

#### Soluzioni
1. controllare finecorsa
2. sostituire relè
3. mandare scheda in assistenza

---

## Codice 101 {#101}
La periferica [47](../../../periferiche/indirizzi.md#indirizzo-47) è assente o guasta.

#### Descrizione
Non è stato ricevuto nessun mesaggio sul bus seriale dalla periferica [47](../../../periferiche/indirizzi.md#indirizzo-47) per più di 200 millisecondi.

#### Cause
1. periferica difettosa
2. periferica diconnessa
3. connessione bus difettosa

#### Soluzioni
1. mandare scheda periferica in assistenza
2. connettere periferica
3. controllare connessione [bus locale](../../../bus_seriali/README.md#bus-locale)

---

## Codice 102 {#102}
La batteria di alimentazione del CEV e braccio per controllo emedamento A3 è guasta.

#### Descrizione

#### Cause

#### Soluzioni

---

## Codice 103 {#103}
Scaduto tempo corsa per impianto a fune a 1 velocità.

#### Descrizione
Dopo il comando di fermata ricevuto con la prima pista, il secondo induttore non si è chiuso entro il tempo stabilito. Si deduce che la cabina non è arrivata al piano.

#### Cause
1.   induttore ID o IS difettoso
2.   cavo di cabina difettoso
3.   accoppiamento piste magnetiche induttore errato
4.   interferenza magnetiche
5.   piste di fermata registrate non correttamente

#### Soluzioni
1. cambiare induttore
2. controllare cavo di cabina
3. assicurarsi che la distanza tra induttore e pista non sia maggiore di 1cm
4. posizionare le piste di fermata con lati opposti (ad esempio una con lato giall ed una con lato nero)
5. assicurarsi che lo spazio di sovrapposizione tra le piste di fermata sia di almeno 2cm, regolare la fermata con i parametri [015](../parametri/temporizzazioni.md#015) e [016](../parametri/temporizzazioni.md#016).

---

## Codice 104 {#104}
[Periferica 46](../../../periferiche/indirizzi.md#indirizzo-46) assente o guasta.

#### Descrizione
La periferica non ha comunicato con la scheda madre per un tempo maggiore a 200ms.

#### Cause
1. periferica difettosa
2. periferica diconnessa
3. connessione bus difettosa

#### Soluzioni
1. cambiare periferica
2. connettere periferica
3. controllare connessione [bus locale](../../../bus_seriali/README.md#bus-locale)

---

## Codice 255 {#255}
Scaduto il timer WDT (watch dog timer).

#### Descrizione
Questo timer interviene in caso il software rimanga bloccato resettando la scheda.

#### Cause
Bug nel software.

#### Soluzioni
Contattare l'assistenza tecnica.
