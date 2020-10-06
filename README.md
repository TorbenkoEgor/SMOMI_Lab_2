## Лабораторная работа №2

При описании нейронных сетей описывались только Conv2D слои. Input, MaxPool2D, Flatten, Dense используются, но не описываются. По умолчанию BATCH_SIZE = 256, lr = 0.000001.

---

# train1.py

Модель использует 2 свёрточных слоя. В свёрточных слоях 8, 8 фильтров соответсвенно.

	tf.keras.layers.Input(shape=(224,224,3)),
	tf.keras.layers.Conv2D(filters=8, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=8, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Flatten(),
	tf.keras.layers.Dense(NUM_CLASSES, activation=tf.keras.activations.softmax)

Тренировочные данные - Синий график

Валидационные данные - Коричневый график

Метрика точности
 
![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_1.png)

Метрика функции потерь

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_2.png)

---

# train2.py

Модель использует 3 свёрточных слоя. В свёрточных слоях 8, 8, 8 фильтров соответсвенно.

	tf.keras.layers.Input(shape=(224,224,3)),
	tf.keras.layers.Conv2D(filters=8, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=8, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=8, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Flatten(),
	tf.keras.layers.Dense(NUM_CLASSES, activation=tf.keras.activations.softmax)

Тренировочные данные - Голубой график

Валидационные данные - Розовый график

Метрики точности

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_3.png)

Метрика функции потерь

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_4.png)

---

# train3.py

Модель использует 3 свёрточных слоя. В свёрточных слоях 32, 16, 8 фильтров соответсвенно.

	tf.keras.layers.Input(shape=(224,224,3)),
	tf.keras.layers.Conv2D(filters=32, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=16, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=8, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Flatten(),
	tf.keras.layers.Dense(NUM_CLASSES, activation=tf.keras.activations.softmax)

Тренировочные данные - Коричневый график

Валидационные данные - Голубой график

Метрика точности

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_6.png)

Метрика функции потерь

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_7.png)

Переобученная сеть

Метрики точности 

Тренировочные данные

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/lab2-3-1.png)

Валидационные данные

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/lab2-3-3.png)

Метрики функции потерь

Тренировочные данные

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/lab2-3-2.png)

Валидационные данные

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/lab2-3-4.png)

---

# train4.py

Модель использует 4 свёрточных слоя. В свёрточных слоях 32, 16, 8, 8 фильтров соответсвенно.

	tf.keras.layers.Input(shape=(224,224,3)),
	tf.keras.layers.Conv2D(filters=32, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=16, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=8, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=8, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Flatten(),
	tf.keras.layers.Dense(NUM_CLASSES, activation=tf.keras.activations.softmax)

Тренировочные данные - Розовый график

Валидационные данные - Зелёный график

Метрика точности

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_8.png)

Метрика функции потерь

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_9.png)
---

# train5.py

Модель использует 4 свёрточных слоя. В свёрточных слоях 32, 32, 16, 8 фильтров соответсвенно.

	tf.keras.layers.Input(shape=(224,224,3)),
	tf.keras.layers.Conv2D(filters=32, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=32, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=16, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=8, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Flatten(),
	tf.keras.layers.Dense(NUM_CLASSES, activation=tf.keras.activations.softmax)

Тренировочные данные - Коричневый график

Валидационные данные - Голубой график

Метрика точности

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_11.png)

Метрика функции потерь

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_12.png)

---

# train6.py

Модель использует 5 свёрточных слоев. В свёрточных слоях 32, 32, 16, 8, 8 фильтров соответсвенно.

	tf.keras.layers.Input(shape=(224,224,3)),
	tf.keras.layers.Conv2D(filters=32, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=16, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=8, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=8, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=8, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Flatten(),
	tf.keras.layers.Dense(NUM_CLASSES, activation=tf.keras.activations.softmax)

Тренировочные данные - Розовый график 

Валидационные данные - Зелёный график

Метрика точности

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_13.png)

Метрика функции потерь

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_14.png)

---

# train7.py

Модель использует 5 свёрточных слоев. В свёрточных слоях 32, 32, 16, 16, 8 фильтров соответсвенно.

	tf.keras.layers.Input(shape=(224,224,3)),
	tf.keras.layers.Conv2D(filters=32, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=32, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=16, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=16, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=8, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Flatten(),
	tf.keras.layers.Dense(NUM_CLASSES, activation=tf.keras.activations.softmax)

Тренировочные данные - Серебристый график

Валидационные данные - Оранжевый график

Метрика точности

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_15.png)

Метрика функции потерь

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_16.png)

---
