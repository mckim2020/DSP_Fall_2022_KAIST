### 2020FALL_DSP
-------------------------
### Filter Design Methods

## 0. 기본기 - 들어가기 앞서
# 0.1 MATLAB function
Matlab 에서는 임의의 n개의 변수를 받아 임의의 k개의 변수를 창출해내는 행위가 가능하다. 
과정은 대부분 다음과 같다. 

# 0.2 도구의 사용
Z-plane 그릴 때:

System 의 frequency response 분석 도구

# 0.3 
## 1. Impulse Invariance Method
# 1.1 Normalization of bands
먼저, Passband과 Stopband 두 경계선을 Td, 즉 sampling interval 로 나누어 주는 Band Normalization을 진행한다. 
# 1.2 Find analog filter prototype
다음으로 Matlab 에 내재되어 있는 함수를 이용하여, 필터의 조건을 충족시키는 최적의 N(order) 값과 Wc(Cutoff Frequency) 값을 구해낸다. 
이후, system function 꼴로 나타내어준다. (Frequency response)
's'
System Function 꼴로 나타내는 방법에는 다음과 같이 크게 두 가지가 있다.

# 1.3 Cutting the edge
필터 설계시, 1.2 단계에서 구한 cutoff frequency, Wc 에 맞추어, system function 을 알맞게 추려낸다. 

# 1.4 Transformation 
Matlab에 내재된 transformation 함수를 이용하여, z transform 의 꼴로 변환된 "new system function"을 얻도록 하자.



## 2. Bilinear Method
# 2.1 Transformation of variables
Laplace transform의 s plane 으로부터 Z transform 의 z plane 으로 옮겨오는 과정이다. 
S-plane 의 y축, 즉 허수 부분은 Z-plane 의 unit circle 에 해당함을 기억하자. 
변환식은 다음과 같다. 

# 2.2 Find analog filter prototype
다음으로 Matlab 에 내재되어 있는 함수를 이용하여, 필터의 조건을 충족시키는 최적의 N(order) 값과 Wc(Cutoff Frequency) 값을 구해낸다. 
이후, system function 꼴로 나타내어준다. (Frequency response)
's'
System Function 꼴로 나타내는 방법에는 다음과 같이 크게 두 가지가 있다.

# 2.3 Cutting the edge
필터 설계시, 1.2 단계에서 구한 cutoff frequency, Wc 에 맞추어, system function 을 알맞게 추려낸다. 

# 2.4 Transformation 
Matlab에 내재된 transformation 함수를 이용하여, z transform 의 꼴로 변환된 "new system function"을 얻도록 하자.
