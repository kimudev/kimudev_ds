## Установка Jupyter Notebook и его расщирения AI-ассистента GigaCode

Установка JN:
```bash
pip install jupyter
show jupyter
```

Установка расширений для JN:
```bash
pip install jupyter_contrib_nbextensions
pip install jupyter_nbextensions_configurator
pip install --upgrade notebook==6.4.12
pip uninstall traitlets
pip install traitlets==5.9.0
jupyter contrib nbextension install --user
jupyter nbextensoins_configurator enable --user
```

Установка AI-ассистена GigaCode файл с расширением необходимо сперва распаковать [файл с расширением](gigacode-jupyter-ext-1.1.176-ext.tar.gz):
```bash
jupyter nbextension install ~/Downloads/gigacode --sys-prefix
jupyter nbextension enable gigacode/main --sys-prefix
```

Также можно поменять исходную тему оформления JN:
```bash
pip install jupyterthemes
jt -t onedork -fs 95 -altp -tfs 11 -nfs 115 -cellw 88% -T #для активации темной темы
jt -r #откатиться к исходной теме
```

Дополнительные настройки в интерфейсе JN:
- Table of Contents - для автоматического создания содержания.
- Hinterland - для автозаполнение кода.
- Code Folding - для возможности сворачивания кода, нажатием на треугольник слева, удобно при объемных функциях.
- Collapsible Headings - то же самое сворачивание только всего содержимого под заголовком.
- ExecuteTime - необходимо для расчёта скорости выполнения окна. Выводит время работы, время окончания и дату запуска.


