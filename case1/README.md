# docker 빌드 하기 (이미지 생성)
-----
Docker 허브에 올라온 ubuntu 이미지를 받습니다.
![](https://github.com/haneal/DockerRepo/blob/master/img/1_docker_pull_ubuntu_latest.png)

이미지가 정상적으로 다운로드 되었는지 확인합니다.
![](https://github.com/haneal/DockerRepo/blob/master/img/2_docker_pull_ubuntu_latest.png)



# docker 컨테이너 만들기 (컨테이너 생성)
-----
컨테이너를 생성하기전에 추후에 네트워크 그룹간 연결을위해 미리 networkgroup을 생성해둡니다.
![](https://github.com/haneal/DockerRepo/blob/master/img/3_1network%20create%20netowrk-group.png)

이제 컨테이너를 생성합니다.
![](https://github.com/haneal/DockerRepo/blob/master/img/4.docker%20%EC%BB%A8%ED%85%8C%EC%9D%B4%EB%84%88%EC%83%9D%EC%84%B1.png)
![](https://github.com/haneal/DockerRepo/blob/master/img/9.run_server_2%EC%83%9D%EC%84%B1.png)



# docker 컨테이너로 접속하기
-----
exec로 접속
![](https://github.com/haneal/DockerRepo/blob/master/img/6.docker_exec.png)

attach로 접속
![](https://github.com/haneal/DockerRepo/blob/master/img/7.attach.png)


# docker 컨테이너간 네트워크 연결
-----

그룹이 생성된것을 확인합니다.
![](https://github.com/haneal/DockerRepo/blob/master/img/3.2.docker-ls.png)
![](https://github.com/haneal/DockerRepo/blob/master/img/3_3_network%20create%20netowrk-group.png)



각각의 컨테이너 websevser 접속해서 ip정보를 확인합니다.
![](https://github.com/haneal/DockerRepo/blob/master/img/8.network_ifconfig_1.png)
![](https://github.com/haneal/DockerRepo/blob/master/img/11.network_ifconfig.png)

ping을 통해 서로간 통신을 확인합니다.
![](https://github.com/haneal/DockerRepo/blob/master/img/13.network_ping_2.png)
![](https://github.com/haneal/DockerRepo/blob/master/img/12.network_ping.png)

