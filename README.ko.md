# Design UI UX — AI Agent Skill for HTML + Tailwind Prototypes

[English](README.md) | [简体中文](README.zh-CN.md) | [繁體中文](README.zh-TW.md) | [日本語](README.ja.md) | 한국어 | [Español](README.es.md) | [Français](README.fr.md) | [Deutsch](README.de.md)

HTML + Tailwind로 UI/UX 프로토타입을 만듭니다. 디자인 참고 자료를 찾고 스타일을 선택한 뒤, 브라우저에서 미리 볼 수 있는 페이지를 제작합니다.

## 설치

npx로 설치합니다. 현재 프로젝트에 설치하는 것을 권장합니다.

```bash
npx skills add ducafecat/design-ui-ux
```

## 사용 방법

### 1. 디자인 참고 자료 찾기

만들 제품, 대상 사용자, 필요한 화면을 설명하는 제품 요구사항 문서(PRD)를 준비한 다음 입력합니다.

```text
/design-ui-ux 샤오홍슈(Xiaohongshu) 스타일의 모바일 UI를 디자인해 주세요.

참고:
docs/prd.md
```

![디자인 방향 검색](images/1795618228981.png)

### 2. 디자인 방향 선택하기

검색 결과에서 마음에 드는 방향을 선택합니다. 적절한 후보가 없다면 추가로 요청합니다.

```text
다른 후보를 보여 주세요.
```

![디자인 방향 선택](images/1795618428611.png)

### 3. 프로토타입 만들기

선택한 참고 자료의 번호(예: B2)를 입력합니다. 이어서 제시되는 스타일 중 하나를 선택합니다. 예를 들어 1번을 선택합니다.

![참고 자료를 선택하고 제안된 스타일을 확인합니다.](images/1795618786169.png)

```text
B2
```

![참고 자료를 선택하고 제안된 스타일을 확인합니다.](images/1795619134358.png)

1번 선택 예시:

```text
1
```

확인 후 프로토타입은 `design/index.html`에 저장됩니다. 브라우저에서 열어 미리 볼 수 있습니다.

![완성된 프로토타입](images/1795620741606.png)

### 4. 화면을 나란히 보기

여러 화면을 한 번에 확인하려면 다음과 같이 입력합니다.

```text
design/index.html의 화면들을 나란히 배치하여 design/平铺.html에 저장해 주세요.
```

저장 위치: `design/平铺.html`

![화면 모아 보기](images/1795620965224.png)

### 5. 여러 시안 비교하기

스타일을 정하기 어렵다면 각 스타일의 홈 화면을 만들어 비교합니다.

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

## 피드백, 유지보수 및 라이선스

개선 사항을 제출하기 전에 [CONTRIBUTING.md](CONTRIBUTING.md)를 읽어 주세요. 변경 이력은 [CHANGELOG.md](CHANGELOG.md), 민감한 문제는 [SECURITY.md](SECURITY.md)를 참고하세요. 재현 가능한 문제는 [GitHub Issues](https://github.com/ducafecat/design-ui-ux/issues)에 보고합니다.

이 프로젝트에는 아직 라이선스가 지정되지 않았습니다. 사용하거나 재배포하기 전에 관련 허가를 확인하세요. 공개 전에 관리자는 코드와 데이터의 출처, 재배포 권한 및 라이선스를 확인해야 합니다. 출처 표기만으로 재배포 권한이 부여되지는 않습니다. [출처 안내](NOTICE.md)를 참고하세요.
