# Introduction
Rapport de projet d'ADSILLH

\pagebreak
# Contenu
Non

Test :

```python
@app.route('/management')
def redirect_management():
    res, client, chambre, conso, bar = liste_client()
    nres, nclient, nchambre, nconso, nbar = select_col_name()
    if isinstance(res, list):
        return render_template("management-board.html", rows_res = res, rows_client = client, rows_chambre = chambre, rows_conso = conso, rows_bar = bar, nres= nres, nclient = nclient, nchambre= nchambre, nconso =nconso, nbar= nbar )
    else: return render_template("management-board.html")

@app.route('/menu_bar')
def redirect_menu_bar(session=session):
    bar = liste_bar()
    return render_template("menu_bar.html", session=session, bar=bar)
```

\pagebreak
# Conclusion
Oui
