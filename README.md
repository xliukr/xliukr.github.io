# Xiaoming Liu CV 사이트

명함 QR 코드로 연결되는 개인 CV 사이트입니다. 서버 없이 `index.html`과 `assets` 폴더만으로 동작하는 정적 사이트이고, GitHub Pages에 올려 **https://xliukr.github.io** 주소로 엽니다.

## 폴더 구성

| 파일 | 역할 |
|---|---|
| `index.html` | 사이트 본문입니다. 내용을 고칠 때는 이 파일만 수정하면 됩니다. |
| `assets/gsph-logo.png` | 서울대학교 보건대학원 로고입니다. 원본 그대로이며, 아래 로고 규칙을 지켜 주세요. |
| `assets/newsreader.woff2`, `assets/instrument-sans.woff2` | 사이트 글꼴입니다. 외부 서버에서 받지 않으므로 중국 등 해외에서도 빠르게 열립니다. |
| `assets/OFL-Newsreader.txt`, `assets/OFL-InstrumentSans.txt` | 글꼴 라이선스 파일입니다. 지우지 마세요. |
| `assets/og-image.png` | 카카오톡, 위챗 등으로 링크를 보낼 때 뜨는 미리보기 그림입니다. |
| `assets/favicon-32.png`, `assets/apple-touch-icon.png` | 브라우저 탭 아이콘과 아이폰 홈 화면 아이콘입니다. |
| `assets/README.txt` | assets 폴더 설명 한 줄입니다. GitHub에서 폴더를 만들 때 씁니다. |
| `README.md` | 이 안내서입니다. 사이트에는 보이지 않습니다. |

공개 CV이므로 전화번호, 주소, 생년월일, 어학 점수는 넣지 않았습니다.

## 1. GitHub Pages에 처음 올리기

GitHub 공식 안내(docs.github.com/en/pages/quickstart)를 따른 절차입니다. GitHub 웹 화면의 **choose your files**로는 폴더를 고를 수 없어서, 파일을 두 번에 나눠 올리고 `assets` 폴더는 GitHub에서 먼저 만든 뒤 그 안에 파일을 올립니다.

**저장소 만들기**

1. github.com에 `xliukr` 계정으로 로그인합니다.
2. 오른쪽 위 **+** 메뉴에서 **New repository**를 누릅니다.
3. Repository name에 `xliukr.github.io`를 정확히 입력하고 **Public**을 선택한 뒤 **Create repository**를 누릅니다. 무료 계정은 공개 저장소에서만 Pages를 쓸 수 있습니다.

**첫 화면 파일 올리기**

4. 저장소 화면에서 **uploading an existing file** 링크(또는 **Add file → Upload files**)를 누릅니다.
5. **choose your files**를 눌러 `index.html`과 `README.md` 두 개를 고르고 **Commit changes**를 누릅니다.

**assets 폴더 만들기**

6. 저장소 첫 화면에서 **Add file → Create new file**을 누릅니다.
7. 파일 이름 칸에 `assets/README.txt`를 입력합니다. `/`를 치는 순간 `assets`가 폴더 이름으로 바뀌면 맞게 된 것입니다.
8. 내용 칸에 `Images and fonts for index.html`이라고 적고 **Commit changes**를 누릅니다.

**assets 폴더 안에 파일 올리기**

9. 저장소 첫 화면에서 `assets` 폴더를 눌러 들어갑니다. 화면 위 경로가 `xliukr.github.io / assets`인지 확인합니다.
10. **Add file → Upload files → choose your files**를 누르고, 내 컴퓨터의 `assets` 폴더 안 파일을 모두 고릅니다. Windows는 `Ctrl + A`, Mac은 `Cmd + A`로 한 번에 고를 수 있습니다. 그다음 **Commit changes**를 누릅니다.

**확인**

11. 저장소 첫 화면에 `index.html`, `README.md`, `assets`가 보이고, `assets` 안에 파일 9개가 있으면 됩니다.
12. **Settings → Pages**(왼쪽 메뉴 Code and automation 안)에서 Source가 **Deploy from a branch**, Branch가 `main` / `/(root)`인지 확인합니다. 다르면 맞춘 뒤 **Save**를 누릅니다.
13. 몇 분 뒤 https://xliukr.github.io 에 접속합니다. 반영까지 최대 10분 정도 걸릴 수 있습니다.

이미 올린 파일을 바꿀 때는 같은 이름의 파일을 같은 위치에 다시 올리면 덮어씁니다.

## 2. 내용 고치기

1. 저장소에서 `index.html`을 누르고 연필 아이콘(**Edit this file**)을 누릅니다.
2. 고친 뒤 **Commit changes**를 누르면 몇 분 안에 사이트에 반영됩니다.
3. 맨 아래 `Updated October 2026`의 날짜도 함께 바꿔 주세요.

편집 화면에서 `Ctrl + F`(Mac은 `Cmd + F`)로 아래 검색어를 찾으면 고칠 곳으로 바로 이동합니다.

| 고칠 내용 | 검색어 | 방법 |
|---|---|---|
| 학력 추가 | `학력 (Education)` | 그 아래 `<li class="entry">`부터 `</li>`까지 한 덩어리를 복사해 맨 위에 붙이고 글자만 바꿉니다. 최신 항목이 위로 갑니다. |
| 경력 추가 | `경력 (Experience)` | 학력과 같은 방법입니다. |
| 수상·장학 추가 | `Awards` 또는 `Scholarships` | 학력과 같은 방법입니다. |
| 기술 추가 | `Software` | `Stata` 뒤에 쉼표로 이어 쓰면 됩니다. 예: `<dd>Stata, R</dd>`. 새 분류는 `<div><dt>…</dt><dd>…</dd></div>` 한 줄을 복사합니다. |
| 연구 관심사 | `Research interests` | 바로 아래 `<p>` 안의 문장을 바꿉니다. |
| 이메일 | `xiaoming@snu.ac.kr` | 나오는 곳을 모두 바꿉니다. |
| 지도교수 | `Soonman Kwon` | 이메일 아래와 학력의 박사 항목, 두 곳입니다. |

새 항목은 아래 틀을 복사해 써도 됩니다.

```html
<li class="entry">
  <p class="when small">2026 – Present</p>
  <div>
    <h3>직함 또는 학위</h3>
    <p>기관 이름</p>
    <p class="meta">보조 설명 (필요 없으면 이 줄을 지우세요)</p>
  </div>
</li>
```

주의할 점이 두 가지 있습니다.

- 글 안의 `&`는 `&amp;`로 써야 합니다. 예: `Health Economics &amp; Policy Lab`
- `<`, `>`, `"` 같은 기호를 지우지 않도록 글자 부분만 바꿔 주세요. 화면이 깨지면 GitHub의 **History**에서 이전 버전으로 되돌릴 수 있습니다.

## 3. TBC 표시

TBC는 To Be Confirmed, 즉 "확인 필요"라는 뜻입니다. 사이트에서 작은 주황색 `TBC`가 붙은 곳은 아직 확인이 필요한 내용입니다.

지금은 한 곳입니다. 경력의 **Program Coordinator**가 공식 직함인지 확인이 필요합니다. 확인되면 `index.html`에서 `tbc`로 검색해 `<span class="tbc" title="공식 직함 확인 필요">TBC</span>` 부분을 통째로 지우세요.

## 4. 로고 사용 규칙 (서울대학교 UI 규정 요약)

출처는 서울대학교 UI 사이트(identity.snu.ac.kr)입니다.

- 로고 파일은 원본 그대로 씁니다. 색이나 비율을 바꾸거나, 자르거나, 늘리거나, 다른 요소를 덧붙이면 안 됩니다.
- 흰 바탕 위에 씁니다. 다크 모드에서도 흰 상자 위에 보이도록 만들어 두었으니 상자의 흰색과 여백을 줄이지 마세요.
- 강한 무늬나 사진 위에 올리지 않고, 상업적 용도로 쓰지 않습니다.
- 서울대 정장(휘장)은 상표로 등록되어 있습니다. 동문이나 외부인은 산학협력단 지식재산관리부(02-880-2216)의 허가가 필요하므로, 졸업 후에는 허가를 받거나 로고를 빼 주세요.

로고를 빼려면 `index.html`에서 `<div class="logo">`부터 그다음 `</div>`까지 지우면 됩니다.

## 5. 색과 다크 모드

휴대폰이 다크 모드이면 사이트도 자동으로 어두운 배색으로 바뀝니다. 색은 `index.html` 위쪽 `<style>` 안에서 바꿀 수 있습니다.

- `:root { … }` 블록: 밝은 화면의 색
- 바로 아래 `@media (prefers-color-scheme: dark)` 블록: 다크 모드의 색

한국어·중국어 이름(유효명, 劉曉鳴)은 휴대폰 기본 글꼴로 표시됩니다.

## 6. 링크 미리보기 그림

`assets/og-image.png`를 같은 이름의 1200×630 그림으로 바꾸면 됩니다. 카카오톡 등은 미리보기를 한동안 저장해 두기 때문에 바뀐 그림이 늦게 보일 수 있습니다.

## 7. 명함 QR 코드

- 주소는 `https://xliukr.github.io`입니다. 저장소 이름을 바꾸지 않는 한 그대로 유지되므로, 내용을 고쳐도 명함을 다시 인쇄할 필요가 없습니다.
- QR 코드는 주소가 그대로 들어간 **정적 QR**을 쓰세요. 중간에 자기 주소를 거치게 하는 동적 QR 서비스는 나중에 유료로 바뀌거나 만료될 수 있습니다.
- 인쇄소에 넘기기 전에 휴대폰 카메라로 찍어 주소가 바로 뜨는지 확인하세요.

## 8. 글꼴 라이선스

Newsreader와 Instrument Sans는 SIL Open Font License 1.1에 따라 무료로 쓸 수 있습니다. 라이선스 파일(`assets/OFL-*.txt`)은 글꼴과 함께 두어야 하니 지우지 마세요.
