# Design UI UX — AI Agent Skill for HTML + Tailwind Prototypes

[English](README.md) | [简体中文](README.zh-CN.md) | [繁體中文](README.zh-TW.md) | [日本語](README.ja.md) | 한국어 | [Español](README.es.md) | [Français](README.fr.md) | [Deutsch](README.de.md)

코딩 도우미에서 쓰는 UI/UX 디자인 스킬입니다. 참고할 디자인과 스타일을 고르면 요구사항에 맞춰 HTML + Tailwind 프로토타입을 만듭니다. 완성된 파일은 브라우저에서 열어 볼 수 있습니다.

## 설치

프로젝트 폴더에서 실행하세요.

```bash
npx skills add ducafecat/design-ui-ux
```

## 사용 방법

### 1. 디자인 참고 자료 찾기

무엇을 만들지, 누가 사용할지, 어떤 화면이 필요한지 알려 주세요. 제품 요구사항 문서(PRD)가 있다면 파일 경로를 함께 적습니다.

```text
/design-ui-ux 샤오홍슈(Xiaohongshu) 스타일의 모바일 UI를 디자인해 주세요.

참고:
docs/prd.md
```

![디자인 방향 검색](images/1795618228981.png)

### 2. 디자인 방향 선택하기

마음에 드는 참고 자료를 고릅니다. 없다면 다른 후보를 요청하세요.

```text
다른 후보를 보여 주세요.
```

![디자인 방향 선택](images/1795618428611.png)

### 3. 프로토타입 만들기

선택한 참고 자료의 번호로 답합니다. 예를 들면:

![참고 자료 선택](images/1795618786169.png)

```text
B2
```

이어서 스타일을 고릅니다.

![스타일 선택지](images/1795619134358.png)

첫 번째 옵션을 고르려면 이렇게 답하세요.

```text
1
```

확인 후 프로토타입은 `design/index.html`에 저장됩니다. 브라우저에서 열어 미리 볼 수 있습니다.

![완성된 프로토타입](images/1795620741606.png)

### 4. 화면을 나란히 보기

모든 화면을 한 페이지에 모아 달라고 요청할 수 있습니다.

```text
design/index.html의 화면들을 나란히 배치하여 design/平铺.html에 저장해 주세요.
```

저장 위치: `design/平铺.html`

![화면 모아 보기](images/1795620965224.png)

### 5. 여러 시안 비교하기

아직 고민된다면 스타일마다 홈 화면을 하나씩 만들어 비교해 보세요.

```text
1, 2, 3, 4번 옵션별로 홈 화면을 하나씩 만들고 design/compare.html에 저장해 주세요.
```

저장 위치: `design/compare.html`

![네 가지 디자인 시안](images/1795619938511.png)

## 환경 요구사항

- 설치에는 Node.js 22.20 이상과 npm / npx가 필요합니다. 생성된 HTML 페이지를 여는 데는 Node.js가 필요하지 않습니다.
- 로컬 데이터 검색에는 Python 3가 필요하며 외부 패키지는 필요하지 않습니다. Python 없이도 디자인 지침에 따라 페이지를 만들 수 있지만 로컬 검색은 사용할 수 없습니다.
- 참고 자료 검색과 화면 확인에는 스크린샷 및 로컬 HTML 미리 보기를 지원하는 브라우저가 필요합니다. 기본은 Ego Lite이며 `ego-browser` 스킬을 별도로 설정해야 합니다. 스킬 설명에 따라 다른 브라우저도 사용할 수 있습니다.
- 제작 중 Tailwind를 컴파일해야 합니다. 최종 HTML을 Node.js, CDN 또는 실행 시 빌드 없이 열 수 있도록 전달 전에 컴파일합니다.

## 피드백과 라이선스

개선 사항을 제출하기 전에 [CONTRIBUTING.md](CONTRIBUTING.md)를 읽어 주세요. 변경 이력은 [CHANGELOG.md](CHANGELOG.md), 민감한 문제는 [SECURITY.md](SECURITY.md)를 참고하세요. 재현 가능한 문제는 [GitHub Issues](https://github.com/ducafecat/design-ui-ux/issues)에 보고합니다.

이 프로젝트는 [MIT 라이선스](LICENSE)로 제공됩니다. 타사 코드, 데이터, 글꼴, 이미지 및 기타 자료에는 각 자료의 라이선스가 적용됩니다. 상위 프로젝트 표기와 출처 기록은 [NOTICE.md](NOTICE.md)를 참고하세요.
