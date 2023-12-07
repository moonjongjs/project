# 깃허브(GitHub) Collaboration(협업)
---

``````
# 다른 사람의 원격 저장소로부터 협업하는 방법
  * Fork, clone, upstream, Pull Request, Merge & Pull
  * 팀장의 깃 저장소(Repository)를 upstream 이라한다.(원본) 
    - https://github.com/moonjongjs/project    
  * fork하고 clone 한 본인 깃주소를 origin 이라한다.(복제본)
    - https://github.com/moonjongjs/project_fork
    - https://github.com/jeungla1303/project_fork2.git

[1] 목차
    1. 메일수신 
       - Moon Jongjs가 귀하를 Moon Jongjs/project에 초대했습니다.
       - @moon Jongjs 님이 Moon Jongjs/project 저장소 에서 공동 작업하도 
         록 귀하를 초대했습니다. 
       - 초대장보기(View invitation) : 클릭 수락
       - 클릭하면 이동한다.       
       - 용어 정리  
       
    2. Fork 클릭 Create a new fork 다른 사람의 프로젝트를 나에게 복제하기
       - fork name 만들기 : project_fork

    3. clone 하기 : origin 생성됨
       $ git clone  https://github.com/javamoonjong/project_fork.git

    4. upstream 저장소 추가하기
       $ git remote add upstream https://github.com/moonjongjs/project

    4. 저장소 확인 하기
       $ git remote -v
       origin  https://github.com/javamoonjong/project_fork.git (fetch)
       origin  https://github.com/javamoonjong/project_fork.git (push) 
       upstream        https://github.com/moonjongjs/project (fetch)   
       upstream        https://github.com/moonjongjs/project (push)  

    4. branch 생성
       $ git branch javamoonjong
       
    5. branch 체크아웃 하기 (javamoonjong)  
       $ git checkout javamoonjong
       Switched to branch 'javamoonjong'

    6. 제작 및 수정 작업
       ...

    7. add
       $ git add .

    8. commit
       $ git commit -m  '프로젝트 제작 및 수정'

    9. push
       $ git push  origin  javamoonjong

         Enumerating objects: 3, done.
         Counting objects: 100% (3/3), done.
         Delta compression using up to 4 threads
         Compressing objects: 100% (2/2), done.
         Writing objects: 100% (2/2), 258 bytes | 129.00 KiB/s, done.
         Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
         remote: Resolving deltas: 100% (1/1), completed with 1 local object.
         remote:
         remote: Create a pull request for 'javamoonjong' on GitHub by visiting:
         remote:      https://github.com/javamoonjong/project_fork/pull/new/javamoonjong
         remote:
         To https://github.com/javamoonjong/project_fork.git
         * [new branch]      javamoonjong -> javamoonjong
       
    10. Pull Request 생성하기
        - 포크한 깃 허브 저장소 : javamoonjong / project_fork
        가. Pull Request(풀요청) 클릭
        나. Compare & pull request(비교 및 풀요청) 클릭
        다. Add a title 제목, Add a description 설명 추가
        라. Create pull request(풀 생성) 클릭
        마. Merge pull request(병합 풀요청) 클릭
        바. Confirm Merge(병합 확인) 클릭
        사. 완료 후 upstream 으로 이동된다. 
        아. 여기는 병합 완료된 upstream 으로 협조 요청한 원본 저장소이다.
        자. 원본 저장소(project)를 클릭 병합된 내용 확인한다.

         



    7. 코드 리뷰 및 Merge Pull Request

    8. origin repository에 변경내용 당겨오기

``````
## upstream 
