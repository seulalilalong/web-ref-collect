---
name: web-ref-collect
description: 「한 번 더 모으기」 — 강사가 준 첫 고르는 판에서 고른 카드(「고른 것 복사」 글)와 내 브리프로 핀터레스트를 한 번 더 모아, 같은 꼴의 맞춤 고르는 판(사이트판 · UI판)을 내 폴더에 짓는다. 크롬의 Claude 확장으로 읽기만 하고, 파이썬 · 노드 같은 프로그램 없이 돈다. "한 번 더 모아 줘", "맞춤 판 만들어 줘", "고른 것 붙여 넣을게요", 「♥ 번호 … pinterest.com/pin/…」 줄이나 「[UI 1차 고른 것]」으로 시작하는 붙여 넣기에서 쓴다.
---

# 한 번 더 모으기 (web-ref-collect)

강사가 준 첫 판에서 고른 카드 + 내 브리프 → **그 취향으로 핀터레스트를 한 번 더 모아** → 같은 꼴의 고르는 판을 수강생의 사이트 폴더에 짓는다.
**사이트 폴더** = 브리프 `01_브랜드브리프.md`가 있는 폴더(보통 `내사이트`, 대개 지금 작업 폴더). 판과 고른 것은 모두 이 폴더 바로 안에 저장한다 — 하위 폴더를 새로 만들지 않는다.
수강생은 비전문가다. 말은 쉬운 한국어 존댓말로, 한 번에 하나씩 묻는다. 어려운 말(UI · 캡차 등)은 한 줄로 풀어 준다.

| 판 | 언제 | 받는 것 | 짓는 파일 | 카드마다 누르는 칸 |
|---|---|---|---|---|
| **사이트판** | 1주 · 첫 사이트 판을 고른 뒤 | 첫 판 「고른 것 복사」 글 + `01_브랜드브리프.md` | `02_맞춤_고르는판.html` | 전체 무드 · 첫 화면 · 넣고 싶은 요소 · ✕ 이건 싫다 + 한 줄 메모 |
| **UI판** | 2주 · 첫 UI 판을 고른 뒤 | 첫 UI 판 글(`[UI 1차 고른 것]`) + 사이트 맞춤 판에서 고른 것 + 브리프 | `03_UI_맞춤_고르는판.html` | 전체 UI 결 · 메뉴 · 버튼 · 카드 · 칸 · 아이콘 · 장식 · ✕ 이건 싫다 + 한 줄 메모 |

- 판 틀: 이 스킬 폴더의 `site-board.html`(사이트판) · `ui-board.html`(UI판). **판 틀은 고치지 않는다** — 맨 위 `window.BOARD = {…}` 한 덩어리만 바꿔 끼운다.
- 검색어 짜는 법: 이 스킬 폴더의 `query-guide.md`.
- 판 맨 앞 묶음은 **첫 판에서 고른 카드 그대로**다(UI판은 첫 UI 판에서 고른 것 + 사이트 맞춤 판에서 고른 것).

## 지키는 것

1. **읽기만.** 핀터레스트에서 검색 결과 페이지를 열고 읽기만 한다. 핀 저장 · 좋아요 · 팔로우 · 댓글 · 메시지 · 버튼 누르기를 하지 않는다. 그림은 내려받지 않는다(판은 `i.pinimg.com` 주소로 그림을 보여 준다).
2. **로그인 · 캡차는 수강생이 직접.** 비밀번호를 받지 않는다. 캡차(「로봇이 아닙니다」 확인)는 대신 넘기지 않는다.
3. **검색어는 먼저 보여 드리고 「좋아요」를 받은 뒤에 모은다.** 몇 장쯤 · 몇 분쯤 걸리는지 먼저 말한다. 다만 걸음 ①의 **크롬 확인(조각 ㉮)과 판 자리 깔기(Write)는 「좋아요」 전에 한다** — 검색이 아니라서 기다리지 않는다(쉬는 시간을 아끼려는 것).
4. **수강생의 원래 탭은 건드리지 않는다.** 새 탭 하나에서만 일하고, 끝나면 그 탭을 닫는다.
5. **판 하나에 모으기는 한 번.** 「한 번 더」는 한 번이다. 다시 모아 달라고 하시면 「강사님께 먼저 여쭤 볼까요?」라고 답한다.
6. **프로그램을 깔거나 돌리지 않는다**(파이썬 · 노드 · 명령어 없음). 쓰는 도구는 Read · Write · Edit, 그리고 Claude in Chrome(`mcp__claude-in-chrome__*`)뿐이다.
7. **검색어에 사적인 것을 넣지 않는다.** 사람 이름 · 주소 · 전화 · 브리프의 「넣지 않을 것」 · 「공개 범위 확인」 중인 이야기는 검색어에 쓰지 않는다. 업종과 느낌 낱말만, 영어로.
8. 같은 크롬 동작이 2~3번 실패하면 되풀이하지 않고 멈춰서 말한다(아래 「멈춤」).

## 걸음 ① 결 읽기 → 검색어 (수강생의 「좋아요」까지)

아래 1~6을 **한 차례에 모두** 한 뒤 수강생에게 묻는다. 사이트판이든 UI판이든 2(크롬 확인)와 5(판 자리)를 건너뛰지 않는다.

1. **읽는다.** 붙여 넣은 글과 `01_브랜드브리프.md`(없으면 어디 있는지 묻는다). UI판이면 사이트 맞춤 판에서 고른 것(`02_사이트레퍼런스_고른것.md` 또는 붙여 넣은 `[사이트 맞춤 판에서 고른 것]` 글)도 읽는다.
   - 첫 사이트 판 글의 꼴: `♥ M127 밝은 회색 바탕 · … https://www.pinterest.com/pin/1080…/ — 메모` (✕ 줄이 있으면 「싫다」).
   - 첫 UI 판 글의 꼴: `[UI 1차 고른 것]` 아래 갈래별 `  ♥ 메01 사이트 이름 (https://사이트주소) — 메모`, `별로:` 아래 `  ✕ …`.
   - 사이트 맞춤 판 글의 꼴: `카드 자세히:` 아래 `- A03 · 전체 무드, 첫 화면 — 메모 · 검색어 「…」 · 핀 https://… · 그림 https://i.pinimg.com/…`.
2. **크롬을 확인하고 첫 판 카드를 읽는다**(쉬는 시간 전에 막힘을 찾으려고 지금 한다).
   - `ToolSearch`로 크롬 도구를 한 번에 불러온다: `select:mcp__claude-in-chrome__tabs_context_mcp,mcp__claude-in-chrome__tabs_create_mcp,mcp__claude-in-chrome__navigate,mcp__claude-in-chrome__javascript_tool,mcp__claude-in-chrome__browser_batch,mcp__claude-in-chrome__tabs_close_mcp,mcp__claude-in-chrome__computer`
   - `tabs_context_mcp`(createIfEmpty: true)를 부른다. 결과에 빈 탭(새 탭)이 있으면 **그 탭을 쓰고**, 없으면 `tabs_create_mcp`로 새 탭을 하나 연다. 그 탭으로 `https://www.pinterest.com/` 를 연다. 수강생이 원래 쓰던 탭에서는 일하지 않는다.
   - 그 탭에서 아래 **조각 ㉮(카드 읽기)** 를 돌린다. `PINS`에 첫 판 ♥ · ✕ 줄의 핀 번호를 넣는다(UI 첫 판처럼 핀이 아닌 카드는 넣지 않는다). 사이트 맞춤 판에서 온 카드는 이미 그림 주소가 있으니 넣지 않는다. **넣을 핀이 하나도 없어도 `PINS = []`로 돌린다** — 로그인 · 권한을 쉬는 시간 전에 확인하려는 것이다.
   - 결과가 `LOGIN`이면 「크롬에서 핀터레스트에 로그인해 주세요. 다 되면 「됐어요」라고 해 주세요」라고 하고 기다린다. `STOP …`이면 「멈춤」으로.
   - 크롬 도구가 아예 없거나 연결이 안 되면: 「크롬이 켜져 있는지, 크롬 오른쪽 위 퍼즐 조각에서 Claude 확장이 켜져 있고 로그인되어 있는지 봐 주세요」라고 안내하고 기다린다(2~3번 안 되면 「멈춤」).
   - 조각이 `Permission denied for JavaScript execution on this domain`으로 막히면: 크롬의 Claude 확장이 이 사이트에서 일해도 된다는 허락이 아직 없는 것이다. 「크롬 오른쪽 위 Claude 확장 창에서 pinterest.com을 허용해 주세요(허락을 묻는 창이 떠 있으면 「허용」). 다 되면 「됐어요」라고 해 주세요」라고 안내하고 기다린다. 대신 다른 길(스크린샷으로 읽기 등)로 돌아가지 않는다.
3. **공통 결 3~5줄을 말로 정리한다.** 고른 카드의 한 줄 설명 · 메모 · 핀 제목에서 되풀이되는 것(바탕색 · 밝기 · 재질 · 사진이냐 그림이냐 · 글자 결 · 짜임)과 브리프의 업종 · 느낌 낱말 셋을 섞는다. 줄마다 근거 카드 번호를 단다. **피할 결** 1~2줄(✕ 카드 · 브리프의 「넣지 않을 것」)도 적는다. 지어 넣지 않는다 — 카드에 없는 결은 쓰지 않는다.
4. **검색어 묶음을 짠다** — `query-guide.md`(검색어 짜는 법)를 따른다.
   - 사이트판: 묶음 4개 × 검색어 4개 = **16개 안팎(많아도 20개)**. 묶음마다 절반 넘게 `website` · `web design` · `landing page` 를 붙인 줄(실제 웹 화면이 나오게).
   - UI판: **부품별 줄** — 메뉴 · 버튼 · 카드 · 칸 · 아이콘 줄마다 2~3개, 모두 **14개 안팎(많아도 18개)**. 장식(테이프 · 우표 · 스티커) 줄은 사이트에서 그런 결을 고른 사람에게만.
5. **판 자리를 먼저 깔아 둔다 — 빠뜨리지 않는다**(쉬는 시간을 아끼려고, 검색어를 보여 드리기 전에 한다). 판 틀(`site-board.html` 또는 `ui-board.html`)을 Read로 읽고, `window.BOARD`만 아래 「판 데이터」 꼴로 바꿔 **Write**로 사이트 폴더에 저장한다. 이때 `groups`는 비워 두고 자리표를 붙인다: `groups: [] /*@@묶음 자리@@*/`. 이름 · 공통 결 · 피할 결 · 맨 앞 묶음(picks)은 지금 채운다. **판 파일 하나만 Write 한 번으로** 저장한다 — 데이터를 따로 담는 임시 파일을 만들지 않는다(수강생 폴더에 남는다).
6. **보여 드리고 묻는다.** 이 꼴로(첫 줄은 5에서 저장한 판 파일 이름 — 저장하지 않았으면 이 물음을 쓰기 전에 5를 먼저 한다):

   > 판 자리를 깔아 두었어요 — `02_맞춤_고르는판.html` (모은 카드는 「좋아요」 뒤에 채워요)
   >
   > **공통 결** (이 결로 한 번 더 모을게요)
   > 1. 따뜻한 크림 바탕에 실 · 털실 사진이 큼직하게 (M127 · M362)
   > 2. …
   > **피할 결** · 어둡고 차가운 바탕 (M210)
   >
   > **검색어 16개 · 묶음 넷**
   > A · 웹사이트 — 뜨개 공방: `knitting studio website` · `yarn shop web design` · …
   > B · …
   >
   > 모으면 250장쯤, **5분 안팎**(길면 8분) 걸려요. 그동안 크롬은 켜 둔 채로 두세요(다른 탭에서 쉬셔도 돼요).
   > 「좋아요」라고 하시면 시작할게요. 바꾸고 싶은 검색어가 있으면 말씀해 주세요.

   (✕ 줄이 하나도 없었다면 끝에 한 줄: 「첫 판에서 싫었던 카드 번호가 있으면 함께 알려 주세요. 없으면 넘어가도 돼요.」)

## 걸음 ② 핀터레스트에서 모으기 (「좋아요」 뒤 — 수강생은 쉬는 시간)

1. ①에서 연 탭을 그대로 쓴다(탭이 없어졌으면 `tabs_context_mcp`로 다시 확인하고 새 탭을 연다).
2. **묶음 하나를 `browser_batch` 한 번으로** 돈다: 검색어마다 `navigate` → `javascript_tool` 짝을 잇는다.
   - 검색 주소: `https://www.pinterest.com/search/pins/?q=` + 검색어(빈칸은 `%20`).
   - 그 탭에서 **처음 한 번만** 조각 ㉯(모으기 설치)를 돌린다. 그 뒤로는 검색어마다 짧은 조각 ㉰만 돌린다.
3. 결과 한 줄을 읽는다.
   - `OK 16 | q=… | 1분 05초째 | 핀번호:그림번호 핀번호:그림번호 …` → 그 검색어의 카드. 받은 `핀번호:그림번호` 줄을 **고치지 말고 그대로** 모아 둔다. 「…초째」는 첫 검색어부터 흐른 시간이다(마지막 검색어의 값 + 판 짓기 1~2분 = 걸린 시간으로 알린다).
   - `EMPTY 0 | q=…` → 결과 없음. 그 검색어는 빼고 다음으로.
   - `NOFN` → 조각 ㉯를 한 번 더 돌린 뒤 이어 간다.
   - `STOP 이유 | …` → 그 자리에서 멈춘다(「멈춤」). 받은 데까지의 카드는 버리지 않는다.
4. 묶음 하나가 끝날 때마다 수강생에게 한 줄: 「A 묶음 61장 · 1/4」.
5. 다 모으면 이번에 쓴 탭을 `tabs_close_mcp`로 **모두** 닫는다(빈 탭이 남았으면 그것도).

## 걸음 ③ 판 짓기

1. **Edit 한 번**으로 판 파일의 `groups: [] /*@@묶음 자리@@*/`를 모은 묶음으로 바꾼다(꼴은 아래). Edit가 안 되면 판 틀을 다시 Read해서 데이터를 다 넣은 판을 Write로 통째로 저장한다.
2. 이렇게 알린다(경로는 실제 경로로):

   > 맞춤 판을 지었어요 — 검색어 16개 · 카드 203장 · 걸린 시간 7분.
   > 파일 탐색기(맥은 Finder)에서 사이트 폴더(`…\내사이트`)의 **02_맞춤_고르는판.html** 을 두 번 눌러 열어 주세요. (경로 한 줄: 실제 전체 경로)
   > 맨 앞 「첫 판」 묶음은 첫 판에서 고르신 카드 그대로예요. 카드마다 칸을 누르고, 다 고르면 아래 **「골라 둔 것 복사」** → 여기에 붙여 넣어 주세요.
   > 고른 것은 이 컴퓨터의 이 브라우저에만 남아요. 다른 브라우저로 열면 비어 보여요.

3. 수강생이 「골라 둔 것」 글을 붙여 넣으면, 글을 **고치지 않고 그대로** 저장한다 — 사이트판은 `02_사이트레퍼런스_고른것.md`, UI판은 `03_UI_고른것.md`. 맨 위에 날짜 한 줄만 더한다. 「첫 화면」이나 「이건 싫다」가 「없음」이면 하나씩만 더 골라 달라고 한 번 청한다(사이트판만).
4. 판이 안 열리고 「판이 열리지 않았어요」가 보인다고 하시면: 판 파일의 `window.BOARD` 부분을 Read로 다시 보고, 쉼표 · 따옴표 · 괄호가 빠진 자리를 Edit로 고친다.

## 판 데이터 (window.BOARD) 꼴

```js
window.BOARD = {
  id: "silgwa-site-1110",          // 저장 열쇠 — 사람 · 판마다 다르게(영문 · 숫자 · 붙임표)
  kind: "site",                    // 사이트판 "site" · UI판 "ui"
  name: "가게(사이트) 이름",
  made: "2026-11-10",
  common: ["공통 결 한 줄 (M127 · M362)", "…"],
  avoid: ["피할 결 한 줄"],
  picks: [                         // 맨 앞 묶음 — 첫 판에서 고른 카드 그대로
    {code: "M127", v: "like", line: "첫 판의 한 줄 설명", memo: "첫 판 메모", pin: "1080301029377855355", img: "e00a8ed08e4910ad35b8052a914ff250"},
    {code: "M210", v: "nope", line: "…", memo: "", pin: "…", img: "…"},
    // UI판: 첫 UI 판 카드(핀이 아님) — 그림 대신 이름과 주소
    {code: "메01", from: "첫 UI 판", v: "like", title: "사이트 이름", memo: "", link: "https://사이트주소"},
    // UI판: 사이트 맞춤 판에서 고른 카드 — 그림 주소를 그대로
    {code: "A03", from: "사이트 맞춤 판", v: "like", memo: "메모", pin: "1052716481653092409", img: "https://i.pinimg.com/736x/ee/8f/28/ee8f….jpg"}
  ],
  groups: [
    {key: "A", name: "웹사이트 · 뜨개 공방", desc: "이 묶음이 무엇을 찾았는지 한 줄", rows: [
      {q: "knitting studio website", c: "1052716481653092409:ee8f2881f44b5a53bb2f91380e51b2e2 469992911137679217:89a738ca409989dcc1de876d83bbb6af"},
      {q: "yarn shop web design", c: "…"}
    ]},
    {key: "B", name: "…", desc: "…", rows: [ … ]}
  ]
};
```

- `rows[].c`에는 조각 ㉰가 돌려준 `핀번호:그림번호` 줄을 **빈칸으로 이어 그대로** 넣는다. 그림 주소 · 카드 번호는 판이 알아서 만든다(A01, A02… / UI판은 UA01…). 같은 그림은 판이 한 번만 보여 준다.
- `img`에는 그림번호(32자리)나 `https://i.pinimg.com/…` 주소 어느 쪽이든 된다. 그림이 없으면 비워 두면 글 카드로 보인다.
- `v`: 첫 판 ♥ = `"like"`, ✕ = `"nope"`. `from`을 비우면 「첫 판」으로 보인다.
- **picks에 넣는 것** — 사이트판: 첫 사이트 판의 ♥ · ✕ 카드 전부(㉮로 읽은 그림번호와 함께). UI판: 첫 UI 판의 ♥ · ✕ 카드 전부(`from: "첫 UI 판"`, 그림 없이 `title` · `link`) + 사이트 맞춤 판에서 고른 카드 전부(`from: "사이트 맞춤 판"`, 「이건 싫다」는 `v: "nope"`). 빼지 않는다.
- 묶음 `key`는 A, B, C… 순서대로. 묶음 이름은 「웹사이트 · …」처럼 무엇을 찾았는지 알아보게.
- 따옴표 안에 `"`를 쓰지 않는다(쓰려면 「」).

## 크롬 조각 (javascript_tool의 text에 그대로 넣는다)

**㉮ 카드 읽기** — 첫 판 핀의 그림 주소 · 제목 · 원래 사이트를 읽는다(걸음 ①). `PINS`만 바꾼다.

```js
await (async () => {
  const PINS = ['1080301029377855355', '1080301029385321598'];
  if (!/pinterest\./.test(location.host)) return 'NOT_PINTEREST';
  if (document.querySelector('input[type="password"]') || !document.querySelector('[data-test-id="header-profile"],[data-test-id="header-avatar"],a[href*="/_saved"]')) return 'LOGIN';
  const out = [];
  for (const id of PINS) {
    try {
      const res = await fetch('/pin/' + id + '/', { credentials: 'include' });
      if (res.status === 429) return 'STOP 요청 제한';
      if (/\/login/.test(res.url)) return 'LOGIN';
      const h = await res.text();
      const img = (h.match(/https:\/\/i\.pinimg\.com\/736x\/[0-9a-f\/]+\.(?:jpg|png|webp|gif)/) || [''])[0];
      const title = ((h.match(/<title[^>]*>([^<]*)<\/title>/) || ['', ''])[1] || '').replace(/\s*\|\s*Pinterest.*$/i, '').slice(0, 80);
      const link = (h.match(/"link":"(https?:[^"]+)"/) || ['', ''])[1];
      out.push(id + ' ' + (img || '그림없음') + ' ' + (link || '-') + ' ' + title);
    } catch (e) { out.push(id + ' 읽기실패'); }
    await new Promise(r => setTimeout(r, 400));
  }
  return 'OK\n' + out.join('\n');
})()
```

**㉯ 모으기 설치 + 첫 검색어 모으기** — 걸음 ②에서 그 탭의 첫 검색어 뒤에 한 번만.

```js
sessionStorage.setItem('wrc-fn', String.raw`(async () => {
  const N = 16;
  const sleep = ms => new Promise(r => setTimeout(r, ms));
  const blocked = () => {
    const cap = [...document.querySelectorAll('iframe[src*="captcha"],iframe[title*="reCAPTCHA"],#captcha')].some(f => {
      if (/size=invisible/.test(f.getAttribute('src') || '')) return false;
      const s = getComputedStyle(f), b = f.getBoundingClientRect();
      return s.visibility !== 'hidden' && s.display !== 'none' && b.width > 50 && b.height > 50;
    });
    if (cap) return '캡차';
    if (document.querySelector('input[type="password"]')) return '로그인 창';
    const t = document.body ? document.body.innerText : '';
    if (/too many requests|너무 많은 요청|unusual activity|비정상적인 활동/i.test(t)) return '요청 제한';
    if (/계정이 (일시 )?정지|account (has been )?suspended|verify your account|계정을 확인해/i.test(t)) return '계정 경고';
    return '';
  };
  const q = new URLSearchParams(location.search).get('q') || '';
  const t0 = +sessionStorage.getItem('wrc-t0') || (sessionStorage.setItem('wrc-t0', Date.now()), Date.now());
  const took = () => { const sec = Math.floor((Date.now() - t0) / 1000); return Math.floor(sec / 60) + '분 ' + (sec % 60) + '초째'; };
  for (let i = 0; i < 20 && !document.querySelector('[data-grid-item="true"]') && !blocked(); i++) await sleep(300);
  let why = blocked();
  if (why) return 'STOP ' + why + ' | q=' + q;
  if (!document.querySelector('[data-grid-item="true"]')) return 'EMPTY 0 | q=' + q;
  let seen = {}; try { seen = JSON.parse(sessionStorage.getItem('wrc-seen') || '{}'); } catch (e) {}
  const got = [];
  for (let r = 0; r < 6 && got.length < N && !why; r++) {
    for (const it of document.querySelectorAll('[data-grid-item="true"]')) {
      if (got.length >= N) break;
      const a = it.querySelector('a[href*="/pin/"]'), m = a && a.getAttribute('href').match(/\/pin\/(\d+)/);
      const img = it.querySelector('img[src*="i.pinimg.com"]');
      if (!m || !img || it.querySelector('video') || /후원|Promoted|Sponsored/.test(it.innerText)) continue;
      const src = (img.getAttribute('srcset') || '').split(',').map(s => s.trim().split(' ')[0]).find(u => u.includes('/736x/')) || img.src;
      const h = src.match(/\/([0-9a-f]{32})\.(jpg|jpeg|png|webp|gif)/);
      if (!h || seen[h[1]] || seen[m[1]]) continue;
      seen[h[1]] = seen[m[1]] = 1;
      got.push(m[1] + ':' + h[1] + (h[2] === 'jpg' ? '' : '.' + h[2]));
    }
    if (got.length < N) { window.scrollBy(0, innerHeight * 1.5); await sleep(900); why = blocked(); }
  }
  try { sessionStorage.setItem('wrc-seen', JSON.stringify(seen)); } catch (e) {}
  return (why ? 'STOP ' + why : 'OK') + ' ' + got.length + ' | q=' + q + ' | ' + took() + ' | ' + got.join(' ');
})()`);
await (0, eval)(sessionStorage.getItem('wrc-fn'))
```

**㉰ 모으기** — 그 뒤 검색어마다(`navigate` 바로 다음).

```js
sessionStorage.getItem('wrc-fn') ? await (0, eval)(sessionStorage.getItem('wrc-fn')) : 'NOFN'
```

- 조각은 검색 결과에서 광고 · 영상 핀 · 이미 받은 그림을 빼고, 검색어 하나에서 새 카드 16장까지 담는다(아래로 조금씩 내리며 읽는다). 탭 하나 안에서 겹친 그림은 두 번 담지 않는다.
- `browser_batch` 예(묶음 A의 앞 두 검색어 — 탭 번호는 실제 번호로):
  `[{"name":"navigate","input":{"tabId":123,"url":"https://www.pinterest.com/search/pins/?q=knitting%20studio%20website"}},{"name":"javascript_tool","input":{"tabId":123,"action":"javascript_exec","text":"<조각 ㉯>"}},{"name":"navigate","input":{"tabId":123,"url":"https://www.pinterest.com/search/pins/?q=yarn%20shop%20web%20design"}},{"name":"javascript_tool","input":{"tabId":123,"action":"javascript_exec","text":"<조각 ㉰>"}}]`

## 멈춤 — 만나면 더 하지 말고 수강생에게 말한다

1. **로그인 창 · 캡차 · 「너무 많은 요청」 · 계정 경고**(조각이 `STOP …`, 또는 화면에 보임) → 바로 멈춘다. 캡차는 대신 넘기지 않는다.
   - 로그인 · 캡차: 「크롬 핀터레스트 탭에서 직접 해 주세요. 다 되면 「이어서」라고 해 주세요」 → 「이어서」를 들으면 **남은 검색어부터** 이어 간다. 같은 날 두 번째로 막히면 이어 가지 않는다.
   - 요청 제한 · 계정 경고: 그날은 더 모으지 않는다. 그때까지 모은 카드로 판을 짓고 「오늘은 여기까지 모았어요. 강사님께 알려 주세요」라고 한다.
2. **크롬 도구가 2~3번 해도 연결되지 않거나 같은 동작이 거듭 실패** → 멈추고, 무엇을 해 봤고 무엇이 안 됐는지 한두 줄로 말한 뒤 강사님을 부르시라고 한다.
3. **로그인 · 결제 · 계정 설정이 필요한 단계** → 수강생이 직접. Claude는 하지 않는다.
4. 판 파일을 저장하지 못하면(Write가 막힘) → 저장 허락 창이 떴는지 여쭙고, 안 되면 강사님을 부르시라고 한다.

## 판 쓰는 법 (수강생에게 알려 줄 것)

- 판은 파일이라 인터넷 주소가 없다. 파일을 두 번 눌러 크롬(또는 엣지)으로 연다.
- 고른 것은 **그 컴퓨터의 그 브라우저**에 남는다. 같은 브라우저로 다시 열면 이어서 고를 수 있다. 다른 브라우저 · 다른 컴퓨터에선 비어 보인다 — 그래서 다 고르면 꼭 「골라 둔 것 복사」.
- 「최종 정리」 탭에서 칸별로 고른 것을 한눈에 본다. 「전부 비우기」는 두 번 눌러야 지워진다.
- 그림을 누르면 핀터레스트 원본 핀이 새 탭으로 열린다. 그림이 안 뜨는 카드는 원본이 지워진 것이라 건너뛰면 된다.
