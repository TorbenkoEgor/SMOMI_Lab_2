## Лабораторная работа №2

При описании нейронных сетей описывались только Conv2D слои. Input, MaxPool2D, Flatten, Dense используются, но не описываются. По умолчанию BATCH_SIZE = 512, lr = 0.000001.

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

Метрики точности

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_3.png)

Метрика функции потерь

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_4.png)

---

# train3.py

Модель использует 3 свёрточных слоя. В свёрточных слоях 16, 8, 8 фильтров соответсвенно.

	tf.keras.layers.Input(shape=(224,224,3)),
	tf.keras.layers.Conv2D(filters=16, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=8, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=8, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Flatten(),
	tf.keras.layers.Dense(NUM_CLASSES, activation=tf.keras.activations.softmax)

Метрика точности

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_6.png)

Метрика функции потерь

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_7.png)

---

# train4.py

Модель использует 4 свёрточных слоя. В свёрточных слоях 16, 8, 8, 8 фильтров соответсвенно.

	tf.keras.layers.Input(shape=(224,224,3)),
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

Метрика точности

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_8.png)

Метрика функции потерь

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_9.png)
---

# train5.py

Модель использует 4 свёрточных слоя. В свёрточных слоях 32, 16, 8, 8 фильтров соответсвенно. BATCH_SIZE = 128.

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

Метрика точности

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_11.png)

Метрика функции потерь

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_12.png)

---

# train6.py

Модель использует 5 свёрточных слоев. В свёрточных слоях 32, 16, 8, 8, 8 фильтров соответсвенно. BATCH_SIZE = 128.

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

Метрика точности

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_13.png)

Метрика функции потерь

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_14.png)

---

# train7.py

Модель использует 5 свёрточных слоев. В свёрточных слоях 16, 8, 4, 4, 4 фильтров соответсвенно.

	tf.keras.layers.Input(shape=(224,224,3)),
	tf.keras.layers.Conv2D(filters=16, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=8, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=4, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=4, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Conv2D(filters=4, kernel_size=3),
	tf.keras.layers.MaxPool2D(),
	tf.keras.layers.Flatten(),
	tf.keras.layers.Dense(NUM_CLASSES, activation=tf.keras.activations.softmax)

Метрика точности

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_15.png)

Метрика функции потерь

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/Screenshot_16.png)

---
