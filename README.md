### Intro

---

**Version Control(VCS)**

- 파일의 변화를 시간에 따라 기록하여 특정 시점의 버전을 다시 불러올 수 있는 시스템
- ex) Git, Mercurial ... 

**Git**

- 개발과정, 소스파일 등을 버전별로 관리할 수 있는 도구

- 히스토리 관리를 통해 개발 과정, 역사를 시간의 흐름을 기준으로 볼 수 있으며 특정 시점으로 복구가 가능

- **분산 버전 관리 시스템**

**Github**

- Git이라는 도구를 응용할 때 필요한 원격 저장소 사이트

- 각족 원격 저장소들의 집합



### Workflow

---

![workflow1](./images/workflow1.png)



![](./images/workflow2.png)



![](./images/workflow3.png)

```
git init 
git add <file name / directory name>
git commit -m "<commit message>"
git remote add origin <remote repository URL>
git push -u origin master
```

- `git init`
  - 현재 디렉토리를 Working Directory로 지정. 일어나는 작업들을 추적하겠다는 의미로 초기화

- `git add <file name / directory name>` 
  - 추적되고 있지 않는 파일들을 스테이지에 올려 추적, 관리 시작
  - `git status`를 통해 현재 상태 확인 가능 (*Untracked*, *modified*)

- `git commit -m "<commit message>"` 
  - 변경 사항을 메시지와 로컬 저장소에 적용
  - `git log`를 통해 커밋 로그들을 확인할 수 있다.

- `git remote add origin <remote repository URL>`  
  - 주어진 URL의 원격 저장소를  `origin` 이라는 이름으로 등록 

- `git push -u origin master` 
  - `origin` 원격 저장소의 `master` 브랜치에 작업 사항을 동기화



### Collaborate

---

**Flow**

![](./images/collaboration.png)