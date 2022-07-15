# Kubernetes workshop test  
<br/>
<br/>

### 답은 메모장에 저장합니다.

### 메모장 이름을 사번-본인의 이름으로 만듭니다. 


<br/>

```
예시) <사번>-장원석
```

1 : 정답은 이것입니다.

2 : 5

3 : redis 이미지

.

.

.


```


### 사전 소스파일 다운로드
```
cd
git clone https://github.com/wsjang619/k8s_workshop
cd ~/k8s_workshop
```

### Quiz setting
```
kubectl create -f workshop-1.yaml
```

1. 현재 Default 네임스페이스의 pod의 개수는 몇개입니까?


2. 1번 문항을 해결하기 위한 명령어는?


3. 생성된 pod 내 컨테이너는 어떤 이미지를 사용합니까?


4. 3번 문항을 해결하기 위한 명령어는?


<br/>

### Quiz setting
```
kubectl create -f workshop-2.yaml
```

5. 현재 Default 네임스페이스 에서 running 상태인 컨테이너의 개수는 몇개입니까?

6. 위에서 만들어진 오브젝트의 문제점은 무엇입니까?

7. 아래 조건을 만족시키는 Deployment를 생성하는 명령어를 쓰세요.

```
name: dp-5
replicas: 3
image: httpd
```

<br/>

### Quiz setting
```
kubectl create -f workshop-3.yaml
```

8. workshop 네임스페이스의 pod 개수는 몇개입니까?

9. 8번 문항을 해결하기 위한 명령어는?

10. 아래 조건을 만족하는 pod 를 alpha 네임스페이스에 생성하는 명령어를 적고, 생성하세요.

```
name: httpd
image: httpd
```

11. red 라는 pod는 어떤 namespace 에 있습니까?

12. 11번 문항을 해결하기 위한 명령어는?

13. Default 네임스페이스의 kubernetes 라는 이름의 service의 유형은 무엇입니까?

14. Default 네임스페이스의 kubernetes 라는 이름의 service 의 target port 는 무엇입니까?

15. 아래 조건을 만족하는 service를 만드는 명령어를 쓰세요.

```
name: workshop-servivce
type: NodePort
targetport: 8080
port: 80
nodeport: 30080
```

<br/>

### Quiz setting
```
kubectl create -f workshop-4.yaml
```


16. 다음 조건을 만족하며 Default 네임스페이스의 svc-pod 라는 이름의 pod와 연결하는 Service를 배포하는 명령어는?
```
port: 80
targetport: 8080
type: ClusterIP
```

17. 16번의 명령으로 Service 를 배포한 뒤, 해당 Service의 셀렉터는 무엇입니까?


18. 17번 문항을 해결하기 위한 명령어는?

<br/>

### Quiz setting
```
kubectl create -f workshop-5.yaml
```

19. 위에서 배포된 오브젝트의 문제점을 쓰세요.

20. 위 문제점을 해결하고, 정상 동작이 확인되는 스크린샷을 첨부하세요.

<br/>

### Quiz setting
```
kubectl create -f workshop-6.yaml
```

21. ns1 네임스페이스에 LimitRange 를 다음 조건에 맞게 생성하고, 생성한 내용에 대한 스크린샷을 첨부하세요.
(hint = ~/k8s_course/lab5/yaml 에 있는 소스파일 참고)
```
min memory : 0.5G
max memory : 1G
maxLimitRequestRatio : 2
default Request memory : 0.7G
default memory: 0.7G
```

22. ns1 네임스페이스에 ResourceQuota 의 제한 중 limit memory 값은 몇입니까?


23. 22번 문항을 해결한 명령어는?
