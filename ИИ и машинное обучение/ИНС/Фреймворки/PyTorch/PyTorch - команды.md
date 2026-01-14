#Фреймворк 

[[Скользящее среднее]]
## Torch

### basic imports

- `import torch` - основной модуль, вкл. поддержку тензоров и операций
- `from torch import nn` - модуль классов для создания НС
- `torch.optim` - алгоритмы оптимизации
- `torch.util.data` - классы обработки данных
### torch.nn
- `nn.Module` - базовый блок, пользовательские слои
- `nn.Linear` - линейное преобразование, используется для создания **FC** слоев
- `nn.Conv2d` - сверточный двумерный слой
- `nn.Sequential` - контейнер для последовательных слоев
- активационные
- `init.xavier_normal_` - инициализация весов с коэффициентом обратно пропорциональным корню из числа нейронов в слое
- `init.kaiming_normal_` - инициализация весов с коэффициентом обратно пропорциональным корню из **половины** числа нейронов в слое
### torch.optim
- `step()` - метод выполнения шага оптимизации
- `zero_grad()` - метод обнуления градиентов перед некст шагом
- `Adagrad` - метод адаптивного накопительного градиента
- `RMSproop` - метод адаптивного градиента с затуханием и EMA
- `Adam` - метод адаптивного градиента с двумя EMA
- `lr_sheduler` - оптимизатор размера learning rate
### torch.util
#### torch.util.data
- `Dataset` - базовый класс для представления набора данных
- `DataLoader` - позволяет загружать датасет пакетами, перемешивать данные, управлять размерами пакетов и загружать их параллельно

## torchvision

### io

- `read_image` - Reads a JPEG, PNG, WEBP, or GIF в Tensor.
- `decode_image` - Detect whether an image is a JPEG, PNG, WEBP, or GIF and performs the appropriate operation to decode the image into a Tensor.
- `encode_ext` - Takes a (list of) input tensor(s) in CHW layout and returns a (list of) buffer(s) with the contents of the corresponding JPEG file(s).
- `decode_ext` - Decode JPEG image(s) into 3 dimensional RGB or grayscale Tensor(s).
- `read_file` - Reads and outputs the bytes contents of a file as a uint8 Tensor with one dimension.
- `write_file` - Writes the contents of an uint8 tensor with one dimension to a file.
### transforms

- 



