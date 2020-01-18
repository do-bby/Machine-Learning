
---
title: "활성화 함수(Activation Funciton)"
categories: 
  - blogging
last_modified_at: 2020-01-18 T18:23:00+09:00
toc: true
---
활성화 함수란?
활성화 함수는 인공지능의 많은 알고리즘에서 다양한 형태로 사용되고 있는데
어떠한 활서오하 함수를 사용하느냐에 따라 출력 값이 달라지기 때문에,
적절한 활성화 함수를 사용하는 것이 매우 중요합니다.
활성화 함수는 어떠한 신호를 입력받아 적절한 처리를 하여 출력해주는 함수인데,
이를 통해 출력된 신호가 다음단계에서 활성화 되는지 결정합니다.

---
>input data -> {activation function} -> output data
---

Step function


활성화 함수에서 가장 기본이 되는 활성화 함수는 step function인데,
그래프 모양이 계단과 같이 생겼습니다.
이 함수는 임계값을 기준으로 활성화 되거나 혹은 비활성화 되는 형태를 보입니다.
식으로 표현했을 때 아래와 같은 식이고,

{% raw %} <img src="https://qkrdbstn15.github.io/assets/img/AF.jpg" alt=""> {% endraw %}

0을 기준으로 출력이 0이거나 혹은 1로 표현되는 것을 볼 수 있는데,
아래는 step function의 그래프 모양이 계단 형태인것을 알 수 있습니다.

{% raw %} <img src="https://qkrdbstn15.github.io/assets/img/AF1.png" alt=""> {% endraw %}

sigmoid function


sigmoid function은 항상 0과 1사이의 값만 가질 수 있도록하는 비선형 함수입니다.
step function은 0, 1 이라는 출력 값만 가졌지만, 
sigmoid function은 이 사이에도 연속적인 출력값이 있는 것으로 봅니다.
미분이 가능하도록 1과 0사이를 이어주고 식으로 표현하면 다음과 같습니다.

{% raw %} <img src="https://qkrdbstn15.github.io/assets/img/SF.png" alt=""> {% endraw %}

{% raw %} <img src="https://qkrdbstn15.github.io/assets/img/SF1.png" alt=""> {% endraw %}


ReLU function

Rectified Linear Unit의 약자로 ReLU는 선형함수입니다.
sigmoid function의 Gradient Vanishing 문제를 해결하기 위해 많이 사용되는데,
여기서 Gradient Vanishing 문제란 0과 1사이의 값을 가지는 sigmoid function에서
아주 작은 값을 가질 경우 0에 가까운 값을 가지게됩니다.
Gradient Descent를 사용해 Back-propagation 시 각 층을 지나며 지속적으로 곱해주는데,
이때 지나는 층이 많을 경우 결국 0으로 수렴하는 문제입니다.
그렇기 때문에 층이 많을 경우 sigmoid가 잘 작동하지 않습니다.

이를 해결하기위해 ReLU가 생겨났는데, 식은 아래와 같습니다.

{% raw %} <img src="https://qkrdbstn15.github.io/assets/img/RU.png" alt=""> {% endraw %}


ReLU의 가장 큰 장점은 Gradient Vanishing문제를 해결할 수 있고,
미분이 간단하게 된다는 것입니다. 그래프 모양은 아래와 같습니다.

{% raw %} <img src="https://qkrdbstn15.github.io/assets/img/RU1.png" alt=""> {% endraw %}
