🐍 스네이크 게임 (HTML/CSS/JS 단일 파일)
키보드 화살표 키(↑ ↓ ← →) 로 조작하는 스네이크 게임입니다.
별도 설치 없이 index.html 하나만으로 실행됩니다.
래핑 모드(벽 통과), 속도 조절, 최고 점수 저장(localStorage) 기능을 제공합니다.

✨ 주요 기능

HTML 파일 단일 구성
화살표 키로 조작
Space: 일시정지/재개
난이도(속도) 조절: 느림 / 보통 / 빠름
래핑 모드 지원
점수 & 최고점수 저장
브라우저 호환성 좋음 (Chrome/Edge/Firefox/Safari)


📸 스크린샷
이미지가 있다면 다음 경로에 업로드 후 사용하세요:
docs/screenshot.png

마크다운 예:
Markdown!screenshot더 많은 선 표시

🚀 실행 방법

저장소를 다운로드하거나 클론합니다.
루트에 있는 index.html 을 더블클릭합니다.
[시작] 버튼을 누르고 화살표 키로 플레이합니다.


🎮 조작 방법





























입력기능↑ / ↓ / ← / →이동Space일시정지/재개시작 버튼게임 시작일시정지 버튼일시정지/재개리셋 버튼게임 초기화

※ 뱀은 정반대 방향(180도 전환) 으로 즉시 움직일 수 없습니다.


⚙️ 옵션

난이도(속도) 선택
래핑 모드 (벽을 통과하여 반대편으로 이동)
최고 점수 저장: localStorage 자동 저장


📁 파일 구조
.
├── index.html          # HTML + CSS + JS 통합 파일
└── docs/
    └── screenshot.png  # (선택) README용 이미지


🛠 커스터마이징
보드 크기 변경
JavaScriptconst COLS = 21;const ROWS = 21;더 많은 선 표시
색상 변경
CSS:root {  --snake: #5de8a3;  --food: #ffd76b;  --bg: #0b0f20;}더 많은 선 표시
속도 기본값 변경
HTML<select id="speedSelect">  <option value="6">느림</option>  <option value="10" selected>보통</option>  <option value="14">빠름</option></select>더 많은 선 표시

🧪 테스트 팁

키 입력이 안 되면 캔버스를 한 번 클릭해 포커스를 주세요.
게임이 너무 빠르거나 느리면 상단 속도 메뉴에서 조정하세요.
최고 점수를 초기화하려면 다음을 실행:
JavaScriptlocalStorage.removeItem('snake_best')더 많은 선 표시



🐞 트러블슈팅

게임이 너무 빠름/느림 → 속도 옵션 변경
벽에서 반대편으로 이어지지 않음 → 래핑 체크
키 입력 지연 → 다른 탭/백그라운드 전환 시 발생 가능(브라우저 표준 동작)


🤝 기여하기
PR, 버그 제보, 개선 아이디어 모두 환영합니다!
추천 브랜치 전략:
main   → 안정 버전
dev    → 개발용
feature/* → 기능 추가

PR 체크리스트:

 브라우저에서 테스트 완료
 README 반영 여부 확인
 변경된 코드에 주석 포함


📜 라이선스
이 프로젝트는 MIT License 하에 배포됩니다.

💡 참고
이 프로젝트는 클래식 스네이크 게임 규칙에서 영감을 받아 제작되었습니다.
