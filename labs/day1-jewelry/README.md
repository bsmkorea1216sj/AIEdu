# 1일차 정적 웹앱 실습

뿌쥬아의 상품 탐색과 구매문의 흐름을 참고한 교육용 페이지입니다. 상품과 그림은 예시이며, 입력은 브라우저에 미리보기로 표시됩니다. [뿌쥬아 자사몰](https://ppujyua.co.kr/)

1. AIEdu 저장소를 VS Code로 클론하고 실습 브랜치를 엽니다.
2. 이 폴더의 `index.html`을 브라우저에서 엽니다. 로컬 Python이 있으면 이 폴더에서 `python -m http.server 8000 --bind 127.0.0.1`을 실행하고 `http://127.0.0.1:8000`에 접속해도 됩니다.
3. 빈 폼을 제출해 상품 선택 안내를 확인합니다. 상품 카드에서 **반지 문의하기**를 누르고, 빈 내용으로 한 번 더 제출해 안내를 확인합니다.
4. **반지 12호 옵션이 있나요?**를 입력하고 제출합니다. 선택한 상품과 문의 내용이 미리보기에 나와야 합니다.
5. Codex에 상품 설명 한 줄을 바꾸도록 요청하고, VS Code에서 변경 내역을 확인한 뒤 같은 테스트를 반복합니다. 실습 브랜치의 변경만 커밋하고 푸시합니다.

Colab에서는 같은 폴더의 노트북을 열고 첫 셀부터 실행합니다. 첫 셀은 GitHub에 올라온 HTML을 읽거나 노트북 옆의 로컬 HTML을 사용합니다.

## Cloud Run 배포

수업용 GCP 프로젝트에 로그인한 다음 이 폴더에서 실행합니다. 아래 명령은 공개 데모용입니다.

```powershell
gcloud run deploy aiedu-jewelry-demo --source . --region asia-northeast3 --port 80 --allow-unauthenticated --project YOUR_PROJECT_ID
```

배포가 끝나면 표시된 서비스 주소를 휴대폰에서 열고 3~4단계를 반복합니다. [Cloud Run 소스 배포 안내](https://cloud.google.com/run/docs/deploying-source-code)
