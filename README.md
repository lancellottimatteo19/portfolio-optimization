# Ottimizzazione di Portafoglio con CVXPY

Ottimizzazione convessa di portafoglio secondo la **Modern Portfolio Theory** di Markowitz, con vincoli realistici.

## Contenuto — [`frontiera_efficiente.ipynb`](frontiera_efficiente.ipynb)

* Portafoglio a **Minima Varianza Globale (GMV)** con `CVXPY`.
* **Frontiera efficiente** con vincolo di concentrazione $w_i \le 0.35$ e senza vendite allo scoperto.
* **Portafoglio tangente** (Sharpe Ratio massimo) con la trasformazione di **Charnes-Cooper**, che rende convesso il problema, e **Capital Market Line**.

## Risultati

Con 5 titoli sintetici e tasso privo di rischio del 2%, il portafoglio tangente ha rendimento atteso 10.74%, volatilità 6.42% e Sharpe Ratio 1.360; il valore coincide con quello trovato esplorando 400 punti della frontiera.

## ▶️ Esecuzione

Serve Python 3.9 o successivo.

```bash
git clone https://github.com/lancellottimatteo19/portfolio-optimization-cvxpy.git
cd portfolio-optimization-cvxpy
pip install -r requirements.txt
jupyter lab
```

I notebook sono salvati con gli output, quindi grafici e risultati si vedono anche direttamente su GitHub.
