## Exercise 2.4

### Question:

시간 간격의 크기 ![equation](https://latex.codecogs.com/svg.latex?\alpha_n) 이 고정된 값이 아니라면 추정값 ![equation](https://latex.codecogs.com/svg.latex?Q_n) 은 이전까지 받은 보상들의 가중 평균이고, 이때 가중치는 식 2.6에서 주어지는 것과는 다르다. 식 2.6과 유사한 일반적인 경우에 있어서 바로 이전 보상에 적용할 가중치는 얼마인가? 시간 간격의 크기와 관련하여 답변해 보라.

### Answer:

<img src="https://latex.codecogs.com/svg.latex?\begin{align*}&space;Q_{n&plus;1}&space;&=&space;Q_n&space;&plus;&space;\alpha_n[R_n-Q_n]&space;\\&space;&=&space;\alpha_nR_n&space;&plus;&space;(1-\alpha_n)Q_n&space;\\&space;&=&space;\alpha_nR_n&space;&plus;&space;(1-\alpha_n)[\alpha_{n-1}R_{n-1}&space;&plus;&space;(1-\alpha_{n-1})Q_{n-1}]&space;\\&space;&=&space;\alpha_nR_n&space;&plus;&space;(1-\alpha_n)\alpha_{n-1}R_{n-1}&space;&plus;&space;(1-\alpha_n)(1-\alpha_{n-1})Q_{n-1}&space;\\&space;&=&space;\alpha_nR_n&space;&plus;&space;(1-\alpha_n)\alpha_{n-1}R_{n-1}&space;&plus;&space;\cdots&space;&plus;&space;\prod_{i=2}^{n}(1-\alpha_i)\alpha_1R_1&space;&plus;&space;\prod_{i=1}^{n}(1-\alpha_i)Q_1&space;\\&space;&=&space;\alpha_nR_n&space;&plus;&space;\sum_{i=1}^{n-1}\prod_{j=i&plus;1}^{n}(1-\alpha_j)\alpha_iR_i&space;&plus;&space;\prod_{i=1}^{n}(1-\alpha_i)Q_1&space;\end{align*}" title="\begin{align*} Q_{n+1} &= Q_n + \alpha_n[R_n-Q_n] \\ &= \alpha_nR_n + (1-\alpha_n)Q_n \\ &= \alpha_nR_n + (1-\alpha_n)[\alpha_{n-1}R_{n-1} + (1-\alpha_{n-1})Q_{n-1}] \\ &= \alpha_nR_n + (1-\alpha_n)\alpha_{n-1}R_{n-1} + (1-\alpha_n)(1-\alpha_{n-1})Q_{n-1} \\ &= \alpha_nR_n + (1-\alpha_n)\alpha_{n-1}R_{n-1} + \cdots + \prod_{i=2}^{n}(1-\alpha_i)\alpha_1R_1 + \prod_{i=1}^{n}(1-\alpha_i)Q_1 \\ &= \alpha_nR_n + \sum_{i=1}^{n-1}\prod_{j=i+1}^{n}(1-\alpha_j)\alpha_iR_i + \prod_{i=1}^{n}(1-\alpha_i)Q_1 \end{align*}" />

시간 간격의 크기 ![equation](https://latex.codecogs.com/svg.latex?\alpha_n) 이 고정된 값이 아닐 경우, 추정값 ![equation](https://latex.codecogs.com/svg.latex?Q_n) 에 대해 바로 이전 보상 ![equation](https://latex.codecogs.com/svg.latex?R_n) 에 적용할 가중치는 시간 간격의 크기 ![equation](https://latex.codecogs.com/svg.latex?\alpha_n) 이 된다.