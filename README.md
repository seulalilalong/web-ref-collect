# web-ref-collect · 한 번 더 모으기

「AI 브랜드 웹사이트 4주 과정」 수강생용 Claude 스킬이에요.
강사가 준 첫 고르는 판에서 고른 카드와 내 브리프를 받아, **그 취향으로 핀터레스트를 한 번 더 모아** 같은 꼴의 맞춤 고르는 판을 내 사이트 폴더에 지어 줍니다.

## 넣는 법 — Claude에게 한마디

Claude 데스크톱 앱의 Code 탭에서 이렇게 말하세요.

> 이 주소의 스킬을 깔아 줘 https://github.com/seulalilalong/web-ref-collect

저장 · 실행 허락 창이 뜨면 「허용」을 눌러 주세요.

---

## Claude가 따를 설치 순서

이 저장소의 파일 넷(`SKILL.md` · `site-board.html` · `ui-board.html` · `query-guide.md`)을 **고치지 않고 그대로** 사용자의 스킬 폴더 `web-ref-collect`에 넣는다.

| 컴퓨터 | 넣을 곳 |
|---|---|
| 맥 | `~/.claude/skills/web-ref-collect/` |
| 윈도 | `%USERPROFILE%\.claude\skills\web-ref-collect\` |

1. **파일은 명령으로 받는다.** 웹 읽기 도구(WebFetch)로 읽어 옮겨 적지 않는다 — 내용이 줄거나 바뀐다.
   - 맥 · 윈도의 Bash(Git Bash):
     ```bash
     d="$HOME/.claude/skills/web-ref-collect"; mkdir -p "$d" && for f in SKILL.md site-board.html ui-board.html query-guide.md; do curl -fsSL "https://raw.githubusercontent.com/seulalilalong/web-ref-collect/main/$f" -o "$d/$f" || echo "실패 $f"; done; ls -l "$d"
     ```
   - 윈도 PowerShell:
     ```powershell
     $d = Join-Path $env:USERPROFILE '.claude\skills\web-ref-collect'; New-Item -ItemType Directory -Force -Path $d | Out-Null; foreach ($f in 'SKILL.md','site-board.html','ui-board.html','query-guide.md') { Invoke-WebRequest -UseBasicParsing -Uri "https://raw.githubusercontent.com/seulalilalong/web-ref-collect/main/$f" -OutFile (Join-Path $d $f) }; Get-ChildItem $d
     ```
2. **확인한다.** 파일 넷이 다 있고, `SKILL.md` 첫 줄이 `---`, 둘째 줄이 `name: web-ref-collect`인지 본다. 하나라도 빠졌으면 한 번 더 받고, 그래도 안 되면 무엇이 안 됐는지 한 줄로 말하고 강사님을 부르시라고 한다.
3. 이미 깔려 있었으면 새 파일로 덮어쓴다(업데이트).
4. 수강생에게 쉬운 말로 알린다: 「깔았어요. 첫 판에서 「골라 둔 것 복사」를 눌러 여기에 붙여 넣으시면 한 번 더 모아 드려요.」 — 이 대화에서 스킬이 보이지 않으면 새 대화를 열면 된다고 덧붙인다.

---

## 쓰는 법

| 언제 | 붙여 넣을 것 | 생기는 파일 |
|---|---|---|
| 1주 · 첫 사이트 판을 고른 뒤 | 첫 판의 「골라 둔 것 복사」 글 (브리프 `01_브랜드브리프.md`는 Claude가 폴더에서 읽어요) | `02_맞춤_고르는판.html` |
| 2주 · 첫 UI 판을 고른 뒤 | 첫 UI 판의 「골라 둔 것 복사」 글 | `03_UI_맞춤_고르는판.html` |

1. 붙여 넣으면 Claude가 **공통 결**과 **검색어**를 보여 드려요. 괜찮으면 「좋아요」.
2. 모으는 동안(5분 안팎) 크롬은 켜 둔 채로 쉬세요.
3. 생긴 판 파일을 두 번 눌러 열고, 카드마다 칸을 누른 뒤 **「골라 둔 것 복사」** → Claude에 붙여 넣기.

## 미리 준비할 것

- Claude Pro 이상 · Claude 데스크톱 앱(Code 탭)
- 크롬(윈도는 엣지)에 Claude 확장 — 같은 계정으로 로그인, 확장에서 `pinterest.com` 허용
- 크롬에서 핀터레스트 로그인 (로그인 · 캡차는 직접 해 주세요. Claude는 비밀번호를 받지 않아요)

## 알아 둘 것

- 핀터레스트는 **읽기만** 해요. 핀 저장 · 팔로우 · 누르기를 하지 않고, 그림도 내려받지 않아요(판은 원래 그림 주소로 보여 줘요).
- 판의 그림은 남의 작품이에요. 취향을 고르는 참고로만 보고, 내 사이트에 그대로 넣지 않아요.
- 고른 것은 그 컴퓨터의 그 브라우저에만 남아요. 다 고르면 꼭 「골라 둔 것 복사」.
