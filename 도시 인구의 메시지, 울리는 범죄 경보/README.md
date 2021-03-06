## **프로젝트 목표**
1979년부터 2019년까지 41년 간 집계된 미국의 **도시 인구 수**와 **범죄**의 회귀분석 프로젝트<br>
### What impact does Population have on crimes?<br>
범죄 발생에 인구 수는 영향력을 미칠까?<br>
<br>
###정부로부터 통고가 날아왔다.<br>
**".. 더 이상 형사 범죄에 전보다 많은 예산을 집행할 수 없습니다.<br>
이렇게나 많은 요원들과 부서가 존재함에도 어째서 범죄 발생 현황은 크게 나아지질 않는 것인지<br>
본 부서의 범죄 예방 및 검거 능력에 많은 의구심이 듭니다.<br>
올해는 작년에 준하여 필요 최소한의 예산만이 집행됩니다.<br>
주어진 자원 안에서 본 부서의 존재 이유를 크게 느낄 수 있는 한 해가 되기를 기대합니다."**<br>  
<br>
### 줄어든 예산 속에서 형사 범죄 예방 및 필요 요원 배치를 위해 오직 인구 수만으로 범죄를 예측하라!
<br>

## **프로젝트 가설**
**주제**:<br>
도시 인구 수를 통한 범죄 발생 예측 시스템 도출<br>
<br> 

**귀무가설**:<br>
인구 수와 형법 범죄 발생건수는 인과관계가 없다.<br>
<br>


**가설 검증 방향**:<br>
1. 연간 범죄율 계산<br>
- 인구 10만 명당 범죄 발생률 연 평균을 구해 범죄 발생 예측 정책 필요성 피력<br>
 - 형법 범죄율은 인구 10만 명당 형법 범죄 발생건수를 나타낸다.<br>
 - 형법 범죄율 계산 방식 = (형법 범죄 발생건수 ÷ 총인구) × 100,000<br>
 - 1979년부터 2018년까지 형법 범죄율 증가추이를 살펴본다.<br>
 - 근 10년 간 형법 범죄 발생률 감소 여부를 확인한다.<br>
 <br> 
2. 인구 수와 범죄 발생 간 상관관계 파악<br>
- scatter plot(산점도) 및 피어슨 상관계수 적용<br>
 - violent crime의 경우<br>
 - property crime의 경우<br>
 <br>

3. 인구 수에 따른 범죄 발생률 인과관계 여부 분석<br>
- 회귀분석(regression)<br>
 - statsmodel의 ols 적용<br>
  - 변수의 정규성: KDE(Kernel Density Estimation)<br>
  - 변수의 선형 상관성: regplot<br>  
  - 변수의 독립성: DW 검정(Durbin-Watson)<br>
- 인구 수에 가장 큰 영향을 받는 형법 범죄 확인<br>
<br>
4. 2019년 인구 수를 통한 형법 범죄 발생 건수 예측<br>
- 최적의 모델 구현<br>
  - sklearn의 LinearRegression 적용<br>
  - sklearn의 DecisionTreeRegressor, RandomForestRegressor 적용<br>
  - sklearn의 GradientBoostingRegressor 적용<br>
  - 모델 예측 정확도 목표 = 90 이상<br>
 <br>
5. 정리<br>
