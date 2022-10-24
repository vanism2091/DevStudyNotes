- [Git](#git)
- [스냅샷 스트림](#스냅샷-스트림)
  - [Delta-based Version Control](#delta-based-version-control)
  - [](#)
- [분산 버전 관리 시스템 (DVCS)](#분산-버전-관리-시스템-dvcs)
  - [작업 모델](#작업-모델)
    - [중앙, 브랜치 저장소](#중앙-브랜치-저장소)
    - [Pull request](#pull-request)

# Git
Git은 컴퓨터 파일의 변경사항을 추적하고 여러 사용자들 간에 해당 파일들의 작업을 조율하기 위한 **스냅샷 스트림** 기반의 **분산 버전 관리 시스템**이다.


# 스냅샷 스트림
## Delta-based Version Control
git과 다른 VCS 사이의 가장 큰 차이점은 깃이 데이터를 다루는 방식이다. 개념적으로, 대부분의 다른 시스템은 정보를 파일 기반 변화의 목록으로 저장한다. 이런 다른 시스템들은(CVS, Subversion, Perforce, Bazaar 등등) 저장한 정보를 파일과 시간이 경과하며 각 파일에서 만들어진 변화의 집합으로 여긴다.(이는 일반적으로 delta-based 버전 컨트롤이라 불린다.)
![Figure 4. Storing data as changes to a base version of each file](https://git-scm.com/book/en/v2/images/deltas.png)

## 
Git은 위와 같은 방식으로 데이터를 다루지 않는다. 대신, 깃은 데이터를 미니어처 파일 시스템의 스냅샷 시리즈로  

# 분산 버전 관리 시스템 (DVCS)
Distributed Version(revision) Control System

## 작업 모델
### 중앙, 브랜치 저장소
공식 저장소로 간주되는 중앙 저장소가 있다. 프로젝트 유지보수자들에 의해 관리된다. 개발자들은 이 저장소를 복제(clone) 후 동일한 로컬 코드 베이스 사본을 만들 수 있다. 중앙 저장소의 소스 코드 변경 사항은 주기적으로 로컬 저장소와 동기화된다.

### Pull request
분산 버전 관리 시스템을 사용하는 소스 코드 저장소의 기여는 일반적으로 풀 리퀘스트(pull request), 즉 머지 리퀘스트 방식으로 이루어진다.




<details closed>
<summary>출처</summary>

* [분산 버전 관리 wiki](https://ko.wikipedia.org/wiki/%EB%B6%84%EC%82%B0_%EB%B2%84%EC%A0%84_%EA%B4%80%EB%A6%AC)
* [깃 wiki](https://ko.wikipedia.org/wiki/%EA%B9%83_(%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4))
* [스냅샷 스트림](https://git-scm.com/book/en/v2/Getting-Started-What-is-Git%3F#:~:text=more%20like%20a-,stream%20of%20snapshots,-.)

</details>
