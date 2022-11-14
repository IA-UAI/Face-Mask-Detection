# Face Mask Detection

Proyecto de detección de Mascarillas con YOLOv7

`export.zip` contiene los pesos del ultimo modelo entrenado

Para el entrenamiento, remplazar el siguiente snippet de codigo con las credenciales de Roboflow[2]

```python
!pip install roboflow

from roboflow import Roboflow
rf = Roboflow(api_key="--------")
project = rf.workspace("----------").project("----------")
dataset = project.version(1).download("yolov7")
```

## Resources

1. [Original YOLOv7 repo](https://github.com/WongKinYiu/yolov7)
2. [How to Train YOLOv7 on a Custom Dataset - Roboflow](https://blog.roboflow.com/yolov7-custom-dataset-training-tutorial/)
