# Instalace

Instalace všeho potřebného není složitá a zabere jen chvíli. Pokud se během ní
přeci jen něco pokazí, popros na Slacku nebo někoho zkušenějšího o radu.

Další kroky počítají s tím, že máš nainstalovaný a funkční Python 3.10-3.12.
Pokud ne, jedna z následujících tří alternativních cest by tě do takové situace měla snadno dovést:

- Obecný návod na instalaci máme k dispozici [v začátečnickém kurzu](https://naucse.python.cz/course/pyladies/sessions/install/). Až budeš vybírat instalátor, sáhni po tom s nejnovější verzí (v okamžiku začátku kurzu 3.12.6), ideálně v 64bitové verzi. Toto je náš preferovaný způsob.

- Máš-li aktualizované Windows 10/11, úplně nejjednodušší je použít instalaci z [Microsoft Store](https://apps.microsoft.com/detail/9ncvdn91xzqp). Toto místo ti otevře i příkaz `python` v příkazové řádce, pokud žádnou jinou instalaci Pythonu ještě nemáš. Nicméně můžeš čekat zádrhele, když začneš instalovat další nástroje Pythonu, které v kurzu nepoužíváme.

- Na MacOS, kromě Homebrew zmiňovaného v návodu začátečnickém kurzu výše, je také jednoduché použít oficiální instalátor z [python.org](https://www.python.org/downloads/macos/). V současnosti je poslední verze 3.12.6 ke stažení [zde](https://www.python.org/ftp/python/3.12.6/python-3.12.6-macos11.pkg).

- Můžeš použít distribuci [Mamba](https://github.com/mamba-org/mamba), která řeší kromě Pythonu samotného i případné další (binární) závislosti a je tak v podstatě nejrobustnějším řešením napříč operačními systémy. Lidé z oblasti data science (včetně některých autorů těchto materiálů) ji rádi používají - sice se tak připravují o práci s "čistým" Pythonem, ale zjednodušují si instalaci některých (zejména výpočetních) knihoven, které závisejí na externích binárních balíčcích. Instalace je jednoduchá, viz [dockumentace](https://mamba.readthedocs.io/en/latest/mamba-installation.html). Na vytváření virtuálních prostředí a instalace balíčků pak slouží příkaz `mamba`, viz [dokumentace](https://mamba.readthedocs.io/en/latest/user_guide/mamba.html).

## Adresář, vytvoření a aktivace virtuálního prostředí

Nejprve si připrav adresář pro ukládání souborů (třeba `pydata`) a v něm si vytvoř
virtuální prostředí.

Pokud nevíš jak na to, kompletní návod je stejně jako pro instalaci Pythonu k dispozici
v [materiálech pro začátečnický kurz](https://naucse.python.cz/2019/pyladies-ostrava-podzim/beginners/venv-setup/).

Po každém spuštění příkazové řádky bude potřeba aktivovat virtuální prostředí, abychom
mohli pracovat s knihovnami a nástroji v něm nainstalovanými.

## Instalace knihoven

Do příkazové řádky s aktivním virtuálním prostředím zadej následující příkaz:

```shell
(venv)$ python -m pip install jupyter pandas matplotlib requests seaborn scipy scikit-learn sqlalchemy plotly xlrd openpyxl
```

Tímto příkazem se do virtuálního prostředí nainstalovaly následující knihovny (a některé další jejich závislosti):

* Jupyter - webové rozhraní pro interaktivní a reprodukovatelnou práci s Pythonem
* Matplotlib - jedna z nejznámějších knihoven pro tvorbu grafů
* Openpyxl - knihovna pro načítání a zápis souborů .xlsx
* Pandas - pro práci s tabulkovými daty
* Plotly - knihovna pro vytváření interaktivních grafů
* Requests - knihovna pro práci s HTTP (webovými a API) požadavky
* Scikit-learn - sbírka nejznámějších algoritmů pro strojové učení
* SciPy - švýcarský nůž pro vědecké výpočty a pokročilou matematiku
* Seaborn - rozšíření pro Matplotlib, které umí vytvořit pokročilejší grafy
* Sqlalchemy - knihovna pro sjednocený, vysokoúrovňový přístup k databázím
* Xlrd - knihovna pro načítání souborů .xls/.xlsx

Pokud kterýkoliv z kroků selže, nebo si jen nebudeš vědět rady, zeptej se na Slacku v kanále `#poradna`, ideálně ještě před zahájením kurzu.

V následující kapitole se podíváme na to, jak Jupyter spustit a jak s ním pracovat.
