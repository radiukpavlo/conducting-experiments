# Налаштування середовища для написання коду з PyTorch

Налаштування власного середовища для програмування методів глибокого навчання може бути досить складним завданням.

Від апаратного забезпечення до програмного, щоб ваш код працював на іншому персональному комп'ютері (ПК) так само, як він працює на вашій машині.

В цьому туторілаі ми розглянемо налаштування середовища на власному локальному/віддаленому ПК. За такого підходу ви матимете більше гнучкості щодо розроблення і тестування вашого коду.

> **Примітка** Також бажано переглянути туторіал з [офіційної документації налаштування PyTorch](https://pytorch.org/get-started/locally/). Якщо ви хочете почати кодувати PyTorch на довгострокову перспективу, вам слід познайомитися з цим туторіалом.

Це **налаштування опирається на операційну систему Windows**. Якщо ви використовуєте macOS або Linux, вам варто звернутися до документації PyTorch.

Це налаштування також **очікує, що ви матимете доступ до графічного процесора NVIDIA (GPU)** (але GPU для цього курсу є необов'язковим).

## Етапи локального налаштування для системи Windows із графічним процесором

1. [Інсталювання Anaconda](https://www.anaconda.com/products/distribution).
Головне тут - це отримати доступ до віртуального середовища `conda` в командному рядку.

2. Створіть теку для матеріалів курсу; ви можете назвати її якзавгодно. Наприклад,

```bash
mkdir ce-course
cd ce-course
```

3. Створіть віртуальне середовище `conda`. Наступна команда створить середовище `course`, яке перебуватиме в теці `anaconda3` на вашому ПК за шляхом `C:\Users\[userName]`. Натисніть `y`, коли команда нижче запитає `y/n?`.

```bash
conda create -n course python=3.8
```

4. Активуйте щойно створене середовище.

```bash
conda activate course
```

5. Інсталюйте необхідні залежні бібліотеки, які вам знадобляться для курсу, наприклад PyTorch і CUDA Toolkit для запуску PyTorch на вашому GPU. Ви можете запустити все це одночасно:

```bash
conda install pytorch==1.13.1 torchvision==0.14.1 torchaudio==0.13.1 -c pytorch # для інсталювання з ПК
# conda install pytorch==1.13.1 torchvision==0.14.1 torchaudio==0.13.1 pytorch-cuda=11.6 -c pytorch -c nvidia
conda install -c conda-forge jupyterlab -y
conda install -c anaconda pip -y
conda install pandas matplotlib scikit-learn -y
```

>**Примітка.** За детялами звертайтесь до [документації з налаштування PyTorch](https://pytorch.org/get-started/locally/).

6. Переконайтеся, що встановлення виконано правильно, запустивши сервер Jupyter Lab:

```bash
jupyter lab
```

7. Після запуску Jupyter Lab, запустіть Jupyter Launcher і виконайте наступний фрагмент коду в комірці.

```python
import pandas as pd
import numpy as np
import torch
import sklearn
import matplotlib

# Перевірте доступ до PyTorch (має вивести тензор)
print(torch.randn(3, 3))

# Перевірте GPU (має повернути True, якщо віртуальний процесор доступний на ПК)
print(torch.cuda.is_available())
```

Якщо наведений вище код працює без помилок, ваше середовище повністю налаштоване та готове до роботи. Натомість якщо ви зіткнулися з помилкою, перейдіть на [сторінку документації з налаштування PyTorch](https://pytorch.org/get-started/locally/).

8. Інсталюйте Visual Studio Code з офіціного сайту за [посиланням](https://code.visualstudio.com/).

9. У Visual Studio Code інсталюйте Python Extension за [посиланням](https://marketplace.visualstudio.com/items?itemName=ms-python.python).

10. Підключіть Visual Studio Code до віртуального середовища `conda`, відповідно до [туторіала](https://code.visualstudio.com/docs/python/environments).
