![image](https://github.com/user-attachments/assets/a0999861-d233-42ec-a89e-70e8cc7e959f)##10주차 과제  
![image](https://github.com/user-attachments/assets/5773d713-e389-43e2-b188-4c802e07e678)
DC 모터의 예시를 보면 OPEN LOOP 시스템에서 지령과 노이즈를 없다고 생각할 시   
![image](https://github.com/user-attachments/assets/4b404f62-a37e-4613-98ec-a23c862b65ee)
와 같은 값이 나오게 된다.  
DISTURBANCE가 발생할 시 외란을 주파수 축으로 가져올 시 $\frac{D}{S}$ 가 나오게 된다.  
FINAL VALUE THEOREM은 에러가 시간이 충분히 지났을 때 어떻게 변하는지 확인할 때 사용한다.    

CLOSE LOOP의 경우에는   
![image](https://github.com/user-attachments/assets/443653c9-6f0a-491d-9150-98e4ad77df55)  
와 같은 GAIN이 나오게 된다.   
이때 LOOP GAIN이 줄어들 수록 노이즈가 줄어들게 된다. 둘은 동시에 줄어들거나 키울 수 없다.
시스템 동작 초반 몇MS동안 TRANSIENT RESOPNSE의 경우 CLOSE LOOP는 빠르게 튀어 지령에 도달하고 OPEN LOOP는  
천천히 도달하게 된다.  
이때 Td가 없을 경우에는 open loop는   
![image](https://github.com/user-attachments/assets/0fc1395f-705f-4228-921a-0e6e3f89f9d2)   
![image](https://github.com/user-attachments/assets/5053cd1d-28a7-4d20-ac0b-e1c031fbe032)  
가 나오게 된다. 이때 Gc(0)은 dc 게인 이다.
close loop의 경우에는  
![image](https://github.com/user-attachments/assets/f9e2c989-6f95-4adb-8e66-1a633165c88b)  
![image](https://github.com/user-attachments/assets/652ba98c-5561-4cd1-8a2a-fe99b95523b6)  
가 나온다.  
#####매트랩코드  
syms는 변수를 그 자체로 사용하겠다는 의미이다.  
positive는 항상 양수이다라는 코드다.  
미분은 diff(f(t))를 이용하고 적분은 int()함수를 이용한다. 이때 tau변수를 이용하게 된다.  
H(t)는 단위계단함수이다. 이는 heaviside(t-a)함수를 이용한다.    
subs는 한 값을 다른 값으로 대체한다는 함수이다.  






