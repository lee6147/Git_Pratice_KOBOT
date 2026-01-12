[내 Git 정리 노션](https://www.notion.so/Git-fdaf6ee12cc14c19baa3a3c9e93331c2?source=copy_link)

1단계: README.md 파일에 링크 넣기 (CLI 방식)
이미 파일을 만드셨더라도, 이 명령어를 입력하면 기존 내용을 덮어쓰면서 링크가 들어갑니다.
Bash
echo "[내 Git 정리 노션](https://www.notion.so/Git-fdaf6ee12cc14c19baa3a3c9e93331c2?source=copy_link)" > README.md

2단계: 변경사항 기록하기 (Add & Commit)
파일을 수정했으니 내 컴퓨터에 "이거 바꿨어"라고 기록을 남깁니다.
Bash
git add README.md
git commit -m "README에 노션 링크 추가"

3단계: 원격 저장소와 싱크 맞추기 (Pull)
아까 발생한 에러를 해결하는 가장 중요한 단계입니다. GitHub에 있는 내용을 내 컴퓨터로 먼저 가져옵니다.
Bash
git pull origin main

참고: 만약 여기서 Merge branch 'main' of ... 같은 창이 뜨면, 당황하지 마시고 :wq를 입력하고 엔터를 치시면 됩니다. (내용을 합치겠다는 뜻입니다.)

4단계: 최종 업로드 (Push)
이제 내 컴퓨터와 GitHub의 히스토리가 합쳐졌으니, 다시 업로드합니다.
Bash
git push origin main

Markdown 링크 문법 요약
나중에 다른 링크를 넣고 싶을 때를 위해 이 규칙만 기억하세요!
종류문법 (README.md 안에 적는 내용)
일반 링크[보여줄 이름](URL주소)
이미지![이미지설명](이미지주소)
이메일[이메일 보내기](mailto:이메일주소)

