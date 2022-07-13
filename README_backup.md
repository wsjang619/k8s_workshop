# Kubernetes workshop test  
<br/>
<br/>

### 답은 다음 명령어로 파일에 저장합니다. (수정 시 vi 편집기 사용하여 편집)

<br/>

```
echo 문제 번호-답 >> ans.txt
```
예시)
```
echo 1-kubectl get nodes >> ans.txt
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



2. 생성된 pod 내 컨테이너는 어떤 이미지를 사용합니까?

<br/>

### Quiz setting
```
kubectl create -f workshop-2.yaml
```

3. 현재 Default 네임스페이스 에서 running 상태인 컨테이너의 개수는 몇개입니까?

4. 위에서 만들어진 오브젝트의 문제점은 무엇입니까?

5. 아래 조건을 만족시키는 Deployment를 생성하는 명령어를 쓰세요.

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

6. workshop 네임스페이스의 pod 개수는 몇개입니까?

7. 아래 조건을 만족하는 pod 를 alpha 네임스페이스에 생성합니다.

```
name: httpd
image: httpd
```

8. red 라는 pod는 어떤 namespace 에 있습니까?

9. Default 네임스페이스의 kubernetes 라는 이름의 service의 유형은 무엇입니까?

10. Default 네임스페이스의 kubernetes 라는 이름의 servic의 target port 는 무엇입니까?

11. 아래 조건을 만족하는 service를 만드는 명령어를 쓰세요.

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


12. 다음 조건을 만족하며 Default 네임스페이스의 svc-pod 라는 이름의 pod와 연결하는 Service를 배포하는 명령어는?
```
port: 80
targetport: 8080
type: ClusterIP
```

13. 12번의 명령으로 Service 를 배포한 뒤, 해당 Service의 셀렉터는 무엇입니까?

<br/>

### Quiz setting
```
kubectl create -f workshop-5.yaml
```

14. 위에서 배포된 오브젝트의 문제점을 쓰세요.

15. 위 문제점을 해결하고 정상 작동하도록 트러블 슈팅하세요.

<br/>

### Quiz setting
```
kubectl create -f workshop-6.yaml
```

16. ns 네임스페이스에 LimitRange 를 다음 조건에 맞게 생성하세요.
(hint = ~/k8s_course/lab5/yaml 에 있는 소스파일 참고)
```
min memory : 0.5G
max memory : 1G
maxLimitRequestRatio : 2
default Request memory : 0.7G
default memory: 0.7G
```

17. ns 네임스페이스에 ResourceQuota 의 제한 중 limit memory 값은 몇입니까?
