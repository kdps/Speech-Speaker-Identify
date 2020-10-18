## 1. 인식유형

### 문장종속(text dependent)

등록된 단어를 사용하여 화자를 인식하여 높은 정확도를 가진 결과물을 가질 수 있음

### 문장독립(text independent)

등록되지 않은 임의의 단어를 사용하여 화자를 인식하여 문장종속에 비해 떨어지는 인식률을 가짐

## 2. 화자인증

### 유사도비 : likelihood ratio (LR)

p(Y | H0)
--------
p(Y | H1)

```Python
import numpy

models = ...

likelihood = numpy.zeros(len(models)) // Gaussian Models
```

### 결정 기준치 : threshold

```Python

models = ...

likelihood = numpy.zeros(len(models)) // Gaussian Models

threshold = numpy.argmax(log_likelihood)
```
