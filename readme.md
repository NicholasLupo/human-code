# Problem Analysis with Pseudolanguage

** 1. Fare la spesa seguendo una lista **

- Nel frigo si inizia a sentire l’eco, perciò è ora di fare rifornimenti!
Visto che dimentico sempre qualcosa, decido di appuntarmi tutto ciò che manca in una lista, così una volta al supermercato, girando tra gli scaffali, posso verificare di aver preso tutto e Ricky non rimane senza crocchette come l’ultima volta, povero! Devo ricordarmi di usare il coupon che scade a fine mese, per il resto dovrebbero bastarmi i contanti che ho in portafogli, sempre se non mi faccio prendere la mano con gli snack extra! -

Creo una lista per fare rifornimento
    - prendo carta e penna
    []
    - inizio a pensare cosa mangiare durante la settimana
        - penso a diverse ricette e a cosa mi serve 🚲
            - apro il frigo o altri luoghi dove deposito il cibo
            - scrivo gli ingredienti che mi servono
                ? SE l'ingrediente che mi serve manca o la quantità è insufficiente
                    * aggiungo alla lista
                    [Uova, Latte, Farina, Cereali, ...]
                : ALTRIMENTI
                    * passo al prossimo ingrediente
    
Vado al supermercato:
    - mi preparo
    - vado a dar da mangiare a Ricky
        - noto che le sue crocchette sono finite
        - prendo la lista
            - aggiungo alla lista le crocchette
            [..., Crocchette per Ricky.]
    - prendo il portafoglio con i contanti
        - noto che ho solamente 50 euro
    - prendo il coupon
        - noto che è valido solo per il Conad
    - guardo sul navigatore il Conad più vicino
        ? SE il tempo di arrivo è inferiore a 5 minuti
            * ci vado a piedi
        : ALTRIMENTI 
            * vado con la macchina

Faccio la spesa e vado in cassa
    - prendo il carrello vuoto
    []
    - entro nel Conad 
    - inizio a girare tra gli scaffali 🚲
        ? SE trovo l'ingrediente annotato nella lista
            * aggiungo al carrello
            [Uova, ...]
        : ALTRIMENTI
            * annoto sulla lista che non c'è
            [<u> Uova </u>, ...]     
        ? SE trovo qualche snack che mi ispira
            ? SE mi faccio prendere dalla mano
                 * aggiungo al carrello
                [Uova, Latte, Patatine, ...]
            : ALTRIMENTI 
                 * continuo il mio giro
        : ALTRIMENTI 
            * continuo il mio giro
        ? SE il contenuto della lista cartacea - <u> gli ingredienti che non ci sono </u> >= contenuto del carrello
            * vado alla cassa
        : ALTRIMENTI 
            * continuo il mio giro

Pago la spesa
    - arrivo alle casse
    - vado alla cassa con meno fila
    - svuoto il carrello sul rullo 🚲
        ? SE il carrello è vuoto
            * vado in fondo alla cassa
        : ALTRIMENTI 
            *continuo a mettere la spesa sul rullo
    - rimetto la spesa nel carrello 🚲
        ? SE la mia spesa è passata dalla cassiera
            * inizio a riempire la spesa
            * chiedo un sacchetto per riempire la spesa 
                ? SE i sacchetti non mi bastano
                    * chiedo un'altro sacchetto
                : ALTRIMENTI 
                    * finisco di riempire i sacchetti
    - pago
        - uso il coupon
        ? SE il prezzo della spesa > contanti nel portafoglio
            * pago con la carta
                ? SE conto sulla carta < prezzo della spesa
                    * lascio gli snack
                        ? SE il prezzo della spesa è ancora troppo elevato
                            * lascio un'altro ingrediente meno indispensabile e lo annoto sulla lista
                            [Uova, Latte, Farina, <u> Succo di frutta </u>, ...]
                        : ALTRIMENTI 
                            * pago
                : ALTRIMENTI 
                    * pago
        : ALTRIMENTI 
            * pago

Torno a casa
    - svuoto la spesa
    - vado a dare da mangiare a Ricky