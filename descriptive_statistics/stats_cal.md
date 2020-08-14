# 기술통계        
### stats_cal tool    
 - SAS 기반 JMP tool(유료 라이선스)의 기술통계 산출 방식을 구현한 것    

## 📄 INPUT / OUTPUT    

## 📄 HOW TO USE     

## 📄 Function    
 - 데이터파일(.xlsx, .csv)에 대해 기술통계 산출               
 1) pandas describe()에서 자동 산출 안 되는 값 7개 더 추가: 첨도, 왜도, 결측치 수, 유일한 값 개수, 범위, 최빈값 등     
 2) 모든 변수에 대해 통계수치 산출. 문자형일 경우 '해당 없음' 반환        
 3) 변수 타입(명목, 비율 여부) 유추해서 찍어줌        
 4) 정수와 실수 알아서 구분함(기존 pandas에서는 실수에 대해 무조건 맞춰짐)           
 5) 숫자 천 단위 , 찍어줌   
 6) 소수점 2자리까지 출력함    
 7) GUI로 만듦(-> exe 전환할 것)     
 
## 📄 Issue        
 1) 파일 읽기 속도 빠르게: pandas, csv, excel(엄청 느림), pickle(가장 빠름 but 행*열 1억 개까지만 가능(?))       
 2) int와 float 구분(기존 pandas에서 int, float 구분 불가. float에 자동 맞춰짐)   
 3) NaN이 포함되어 있는 경우 처리 - NaN 제외 후 기술통계 산출       
 4) 해당 변수가 명목/서열/등간/비율 중 어디에 속하는지 구분    
 5) 첨도의 산출 방식: 데이터 개수가 3개 넘어야 됨   
 6) pandas 자체의 장점을 최대한 활용할 것(프레임 단위로 한 번에 계산 가능) -> NaN이 있을 때 dropna를 언제해야할 것인지    
 7) 최빈값 산출 수정 및 속도 처리 -> 속도 빠르게 해야함                
 8) 대용량 데이터에 대한 기술통계 처리 속도 빠르게 하기    
 

## 📄 Simple GUI Application
![image](https://user-images.githubusercontent.com/44013936/90158945-a3d50380-ddca-11ea-81dc-941d534d2b69.png)    

* (ex) 결측치가 없는 dataframe   
-input    
![image](https://user-images.githubusercontent.com/44013936/90232698-06281580-de58-11ea-88ae-57cfa5b072b8.png)     

-output    
![image](https://user-images.githubusercontent.com/44013936/90232799-222bb700-de58-11ea-8619-0f9efabef581.png)    

* (ex) 결측치가 있는 dataframe    
-input
![image](https://user-images.githubusercontent.com/44013936/90232489-bb0e0280-de57-11ea-8228-3b28aec0a225.png)    

-output    
![image](https://user-images.githubusercontent.com/44013936/90232628-eb55a100-de57-11ea-8113-c3cd437c3ef7.png)    

-[코드 링크](https://github.com/sohyunwriter/ai-tech-archive/blob/master/descriptive_statistics/stats_cal.py)    
