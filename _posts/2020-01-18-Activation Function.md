
---
title: "Ȱ��ȭ �Լ�(Activation Funciton)"
categories: 
  - blogging
last_modified_at: 2020-01-18 T18:23:00+09:00
toc: true
---
Ȱ��ȭ �Լ���?
Ȱ��ȭ �Լ��� �ΰ������� ���� �˰��򿡼� �پ��� ���·� ���ǰ� �ִµ�
��� Ȱ������ �Լ��� ����ϴ��Ŀ� ���� ��� ���� �޶����� ������,
������ Ȱ��ȭ �Լ��� ����ϴ� ���� �ſ� �߿��մϴ�.
Ȱ��ȭ �Լ��� ��� ��ȣ�� �Է¹޾� ������ ó���� �Ͽ� ������ִ� �Լ��ε�,
�̸� ���� ��µ� ��ȣ�� �����ܰ迡�� Ȱ��ȭ �Ǵ��� �����մϴ�.

---
>input data -> {activation function} -> output data
---

Step function


Ȱ��ȭ �Լ����� ���� �⺻�� �Ǵ� Ȱ��ȭ �Լ��� step function�ε�,
�׷��� ����� ��ܰ� ���� ������ϴ�.
�� �Լ��� �Ӱ谪�� �������� Ȱ��ȭ �ǰų� Ȥ�� ��Ȱ��ȭ �Ǵ� ���¸� ���Դϴ�.
������ ǥ������ �� �Ʒ��� ���� ���̰�,

{% raw %} <img src="https://qkrdbstn15.github.io/assets/img/AF.jpg" alt=""> {% endraw %}

0�� �������� ����� 0�̰ų� Ȥ�� 1�� ǥ���Ǵ� ���� �� �� �ִµ�,
�Ʒ��� step function�� �׷��� ����� ��� �����ΰ��� �� �� �ֽ��ϴ�.

{% raw %} <img src="https://qkrdbstn15.github.io/assets/img/AF1.png" alt=""> {% endraw %}

sigmoid function


sigmoid function�� �׻� 0�� 1������ ���� ���� �� �ֵ����ϴ� ���� �Լ��Դϴ�.
step function�� 0, 1 �̶�� ��� ���� ��������, 
sigmoid function�� �� ���̿��� �������� ��°��� �ִ� ������ ���ϴ�.
�̺��� �����ϵ��� 1�� 0���̸� �̾��ְ� ������ ǥ���ϸ� ������ �����ϴ�.

{% raw %} <img src="https://qkrdbstn15.github.io/assets/img/SF.png" alt=""> {% endraw %}

{% raw %} <img src="https://qkrdbstn15.github.io/assets/img/SF1.png" alt=""> {% endraw %}


ReLU function

Rectified Linear Unit�� ���ڷ� ReLU�� �����Լ��Դϴ�.
sigmoid function�� Gradient Vanishing ������ �ذ��ϱ� ���� ���� ���Ǵµ�,
���⼭ Gradient Vanishing ������ 0�� 1������ ���� ������ sigmoid function����
���� ���� ���� ���� ��� 0�� ����� ���� �����Ե˴ϴ�.
Gradient Descent�� ����� Back-propagation �� �� ���� ������ ���������� �����ִµ�,
�̶� ������ ���� ���� ��� �ᱹ 0���� �����ϴ� �����Դϴ�.
�׷��� ������ ���� ���� ��� sigmoid�� �� �۵����� �ʽ��ϴ�.

�̸� �ذ��ϱ����� ReLU�� ���ܳ��µ�, ���� �Ʒ��� �����ϴ�.

{% raw %} <img src="https://qkrdbstn15.github.io/assets/img/RU.png" alt=""> {% endraw %}


ReLU�� ���� ū ������ Gradient Vanishing������ �ذ��� �� �ְ�,
�̺��� �����ϰ� �ȴٴ� ���Դϴ�. �׷��� ����� �Ʒ��� �����ϴ�.

{% raw %} <img src="https://qkrdbstn15.github.io/assets/img/RU1.png" alt=""> {% endraw %}
