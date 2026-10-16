# CASTELIER — 캐릭터 스튜디오

캐릭터 선택 화면과 상세 페이지를 꾸미는 정적 웹 앱입니다.

## 실행

```sh
python3 -m http.server 55271 --directory dist
```

브라우저에서 http://localhost:55271 을 엽니다. 별도 빌드나 패키지 설치가 필요하지 않습니다.

## 파일

- `dist/index.html`: 페이지 구조
- `dist/app.js`: 캐릭터 관리, 내용·디자인 편집, 저장 및 HTML 내보내기
- `dist/style.css`: 화면 디자인과 반응형 스타일
- `dist/export-kit.json`: HTML 다운로드에 사용하는 소스·이미지 묶음
- `dist/stock-sources.json`: 사용한 소재의 출처

정적 호스팅의 게시 디렉터리는 `dist`로 설정합니다.

사용자 편집 내용은 브라우저에 저장됩니다. GitHub 푸시만으로 브라우저의 개인 편집 데이터가 복사되지는 않습니다. 완성한 화면은 앱의 HTML 다운로드 기능으로 내보낼 수 있습니다.
