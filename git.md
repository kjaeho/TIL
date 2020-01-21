# Git

1. git 시작하기

   ```sh
   $ git init
   ```

이제부터 해당 디렉토리를 git으로 관리하겠다!

2. 상태 확인하기

   ```sh
   $ git status
   ```

   관리하지 않는 파일들이 빨간색으로 표현됨, 무대로 올리려면 git add로 올려야함

3. 스테이지에 올리기

   ```sh
   $ git add 파일명
   ```

초록색으로 변하고 앞에 new file이 뜨게됨

4. 커밋하기(사진찍기)

```sh
$ git commit -m '메세지'
```

-는 보통 옵션을 뜻한다 (shell script에서)

5. 기록 확인하기

   ```sh
   $ git log
   ```

6. 리모트(원격 저장소) 등록하기

   ```csharp
   git remote add orgin 원격저장소 수소
   ```

7. 파일 푸쉬하기(업로드)

   ```sh
   $ git push origin master
   ```

   