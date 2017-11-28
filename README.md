# jenkins_docker
Jenkins Using Docker For Android 

## 해당 디렉토리에서 빌드

	$ docker build -t ubuntu-jenkins .
	

빌드가 성공적으로 실행이 되면 Successfully built [commit name] 가 출력

## 만들어진 이미지를 확인
	$ docker images

	$ cd ~
	$ mkdir jenkins_home
	$ sudo chown 1000:1000 jenkins_home
	
## Docker Run
	$ docker run --name ubuntu-jenkins -p 8080:8080 -p 50000:50000 -v ~/jenkins_home:/var/jenkins_home ubuntu-jenkins
	
### 확인은 
	http://localhost:8080/

