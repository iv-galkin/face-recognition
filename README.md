# Система распознавания лиц с ArcFace и Identification Rate Metric

---

### Цель проекта
Познакомиться с задачей распознавания лиц, функцией потерь ArcFace, метрикой Identification Rate, построить свой пайплайн для решения этой задачи.

### Постановка задачи
Допустим, некоторая компания хочет разработать систему распознавания лиц, чтобы применять ее в своем офисе. Например, чтобы сотрудники могли сканировать лицо вместо прикладывания id-карточек к турникетам при входе. Или для обеспечения безопасности в офисе. 

Таким образом, нужна система, которая может принимать на вход фото, полученное с камер наблюдения, и идентифицировать на фото сотрудника. Такая система должна уметь работать в случаях, когда лица людей запечатлены крупным или мелким планом, когда они чуть повернуты или наклонены, и когда на одном кадре с камеры находятся несколько лиц.

Написанный пайплайн может использоваться, например, для решения описанной задачи, а также для ряда других задач, где необходимо распознавать лица. 

### Проблема, которую решает проект
Система распознавания лиц может заменить традиционные методы контроля доступа (например, ID-карты), повысить уровень безопасности в офисах и обеспечить автоматизированный анализ видеопотоков с камер наблюдения.

### Что я узнал в ходе выполнения
В процессе работы над проектом были изучены:
- Функция потерь ArcFace и ее преимущества перед классической Cross Entropy.
- Метрики качества распознавания лиц, в частности Identification Rate.
- Построение пайплайна для распознавания лиц, включая детекцию, выравнивание и классификацию.

---

## Установка

**Клонирование репозитория:**
   ```bash
   git clone https://github.com/iv-galkin/face-recognition.git
   ```
Colab%20Notebooks/Face_Recognition_CE_Loss_and_ArcFace_loss.ipynb
Colab%20Notebooks/Full_Face_Recognition_Pipeline.ipynb
Colab%20Notebooks/Identification_Rate_Metric.ipynb

---

## Подробности 
- Цикл обучения моделей подробно описан в ноутбуке [Открыть ноутбук Face Recognition](Colab%20Notebooks/Face_Recognition_CE_Loss_and_ArcFace_loss.ipynb)
- Реализация Identification Rate Metric и её подсчёт описан в [Открыть ноутбук Identification Rate](Colab%20Notebooks/Identification_Rate_Metric.ipynb)
- Обучение нейросети на задачу поиска ключевых точек и применение полного пайплайна для распознавания лиц смотреть в [Открыть ноутбук Face Recognition Pipeline](Colab%20Notebooks/Full_Face_Recognition_Pipeline.ipynb)

--- 

## Литература 
- [ArcFace: Additive Angular Margin Loss for Deep Face Recognition](https://arxiv.org/pdf/1801.07698.pdf)
- [InsightFace: 2D and 3D Face Analysis Project](https://github.com/deepinsight/insightface)
- [PyTorch Data Loading Tutorial](https://pytorch.org/tutorials/beginner/data_loading_tutorial.html)
- [Обзор методов распознавания лиц](https://habr.com/ru/companies/ntechlab/articles/531842/)
