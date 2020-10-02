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
 
![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/NN1-A-88.png)

Метрика функции потерь

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/NN1-L-88.png)

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

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/NN2-A-1688.png)

Метрика функции потерь

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/NN2-L-888.png)

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

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/NN3-A-1688.png)

Метрика функции потерь

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/NN3-L-1688.png)

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

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/NN4-A-16888.png)

Метрика функции потерь

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/NN4-L-16888.png)
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

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/NN5-A-321688.png)

Метрика функции потерь

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/NN5-L-321688.png)

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

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/NN6-A-3216888.png)

Метрика функции потерь

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/NN6-L-3216888.png)

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

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/NN7-A-168444.png)

Метрика функции потерь

![Image alt](https://github.com/TorbenkoEgor/SMOMI_Lab_2/blob/master/logs/NN7-L-168444.png)

---
