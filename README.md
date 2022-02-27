# Kubernetes workshop test  

  
## 답은 다음 명령어로 파일에 저장합니다. (수정 시 vi 편집기 사용하여 편집)

```
echo 문제 번호-답 >> ans.txt
```
예시)
```
echo 1-kubectl get nodes >> ans.txt
```


## 사전 소스파일 다운로드
```
cd
git clone https://github.com/wsjang619/k8s_workshop
cd ~/k8s_workshop
```

## Quiz setting
```
kubectl create -f workshop-1.yaml
```

1. 현재 Default 네임스페이스의 pod의 개수는 몇개입니까?



2. 생성된 pod 내 컨테이너는 어떤 이미지를 사용합니까?


## Quiz setting
```
kubectl create -f workshop-2.yaml
```

3. 현재 Default 네임스페이스 에서 실행중인 컨테이너의 개수는 몇개입니까?

4. 위에서 만들어진 오브젝트의 문제점은 무엇입니까?

# 7. 아래 조건을 만족시키는 Deployment를 생성하는 명령어를 쓰세요.

```
name: dp-12
replicas: 3
image: httpd
```

## Quiz setting
```
kubectl create -f workshop-3.yaml
```

# 8. workshop 네임스페이스의 pod 개수는 몇개입니까?

# 9. 아래 조건을 만족하는 pod 를 alpha 네임스페이스에 생성합니다.

```
name: redis
image: redis
```

# 10. red 라는 pod는 어떤 namespace 에 있습니까?

# 11. kubernetes 라는 이름의 service의 유형은 무엇입니까?

# 12. kubernetes 라는 이름의 servic의 target port 는 무엇입니까?

# 13. 아래 조건을 만족하는 service를 만드는 명령어를 쓰세요.

```
name: workshop-servivce
type: NodePort
targetport: 8080
port: 80
nodeport: 30080
```


## Quiz setting
```
kubectl create -f workshop-4.yaml
```


# 14. svc-pod 라는 이름의 pod와 연결하는 ClusterIP 유형의 Service를 배포하는 명령어는?



## Quiz setting
```
kubectl create -f workshop-5.yaml
```

# 15. 위에서 배포된 오브젝트의 문제점을 쓰세요.

# 16. 위 문제점을 해결하고 정상 작동하도록 트러블 슈팅하세요.
