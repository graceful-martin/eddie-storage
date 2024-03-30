# 파일공유 서비스 

## 요구사항
1. 공유 웹 화면에 들어가면 다음 폼이 보이고
- 공유할 파일
- 유효시간(분)
- 최대 다운로드 횟수
- 업로드 버튼
- [업로드] 버튼을 누르면 파일 업로드를 마친 뒤에 고유한 공유 URL이 화면에 출력

2. 해당 URL을 조회하면 파일 다운로드
- 유효시간 초과와 최대 다운로드 횟수를 초과하면 에러 메시지

3. 기타 
- 서버 설정에서 최대 파일 크기를 지정할 수 있고 이를 초과하면 업로드 실패 파일은 S3, CDN, 서버 디스크 어디든 저장해도 좋습니다.

## 아쉬운 점
- 기능 단위로 PR을 작성을 못했습니다.
- 테스트 하나가 깨지는데 원인을 찾지 못해서 제출 후 여쭤보려합니다.

## 추가
- application.yml 은 gitignore 처리했습니다.

## 배포
- 배포는 Netlify를 통해 진행했습니다. 