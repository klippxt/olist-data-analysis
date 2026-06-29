# Анализ данных на датасете Olist

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-150458?logo=pandas&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-notebook-F37626?logo=jupyter&logoColor=white)

Серия учебных работ по анализу данных (курс Python и анализ данных, ИТМО) на датасете бразильского e-commerce Olist.

## Работы

**[lab1 — NumPy: векторизация](olist-data-analysis/lab1_numpy_vectorization.ipynb)**
Векторизованные вычисления вместо циклов: скидки через `np.select`, объёмный вес товаров, выручка через скалярное произведение, поиск аномальных цен по правилу 3σ. Бенчмарк цикла против векторизации (`%timeit`), ускорение примерно в 50 раз.

**[lab2 — pandas: очистка и индексация](olist-data-analysis/lab2_pandas_cleaning.ipynb)**
Типизация дат, дедупликация отзывов по `order_id` с сохранением последнего, нормализация текста (lower, regex), корректная работа со строковыми zip-кодами, маски и выборки по условиям, `set_index` и доступ по метке.

**[lab4 — Временные ряды и SLA](olist-data-analysis/lab4_time_series_sla.ipynb)**
Срок доставки в рабочих днях, анализ просрочек (SLA breach), дневная выручка на непрерывной сетке дат, пиковые часы заказов по дням недели. С графиками.

**[lab5 — Визуализация и когорты](olist-data-analysis/lab5_visualization_cohorts.ipynb)**
Hexbin и KDE связи цены и стоимости доставки, скользящие 30-дневные μ/σ и обнаружение аномалий по Z-score, матрица активности, когортная матрица удержания. Seaborn, matplotlib, gridspec.

## Данные

Публичный датасет [Brazilian E-Commerce by Olist](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) (Kaggle). В репозиторий не включён из-за размера. Скачайте с Kaggle и положите csv-файлы рядом с ноутбуками.

Ноутбуки сохранены с выводами, поэтому графики и таблицы видны прямо на GitHub без запуска.

## Запуск

```bash
pip install pandas numpy matplotlib seaborn jupyter
jupyter notebook
```

## Стек

Python, pandas, NumPy, Matplotlib, Seaborn, Jupyter.
