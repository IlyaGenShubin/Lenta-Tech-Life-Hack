**Общая архитектура**

Решение представляет собой многоступенчатый конвейер (pipeline) для автоматического обнаружения и распознавания ценников на видео с последующей идентификацией товаров из базы данных.
1) Первая YOLO модель детекрирует ценники на стеллажах
2) Вторая YOLO модель детекрирует области на ценниках
3) EasyOSR распознаёт текст на этих областях
4) Bge-m3 + Faiss поиск по базе данных
5) Формируется итоговый csv файл с распознными ценниками

**Файлы:**
1) [веса YOLO_1](https://drive.google.com/file/d/1iJBC9lWumtUuO-T0jCUkD7AmC-_JR3gQ/view?usp=sharing)
2) [веса YOLO_2](https://drive.google.com/file/d/17SwJcT2gs5EJRC5wdM0AYvf9Vm4aWO4F/view?usp=sharing)
3) [база данных](https://drive.google.com/file/d/15_YUr0U81VOGE_Blta0lzOUE-_Pv_mvz/view?usp=sharing)
4) [тестовое видео](https://drive.google.com/file/d/13ZgC9q7dpet-Uh4jlvhpiSED9STayuBx/view?usp=sharing)
5) [итоговый файл](https://drive.google.com/file/d/16lQdUg7Vw39tMnHFC0ACWrGJDWuOfMZH/view?usp=sharing)
