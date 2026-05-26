# Contributing · 기여 방법

*English follows Korean. · 영문은 한국어 다음에 이어집니다.*

---

이 문서는 빠띠가 만들어온 디지털 민주주의의 기능과 프로그램을 기록한 **살아있는 문서**입니다. 정적인 목록이 아니라, 빠띠가 새로운 기능을 만들면 추가되고 더 정확한 설명이 제안되면 반영되는 문서입니다. 수정·추가·번역 기여를 환영합니다.

## 기여할 수 있는 것

- **오류 정정** — 사실과 다른 설명, 오탈자, 깨진 링크.
- **설명 개선** — 더 정확하거나 명료한 표현 제안.
- **상태 갱신** — 기능의 구현 상태가 바뀌었을 때 (아래 상태 표시 참고).
- **새 항목 추가** — 아직 기록되지 않은 빠띠의 기능이나 프로그램.
- **번역 개선** — 한국어·영어 표현을 더 자연스럽게 다듬기.

## 기여하는 법

1. [GitHub Issue](https://github.com/parti-coop/digital-democracy-100/issues/new)로 제안하거나, 직접 고칠 수 있다면 Pull Request를 보내 주세요.
2. 작은 정정은 Issue 없이 바로 PR을 보내도 좋습니다. 새 항목 추가나 큰 구조 변경은 Issue로 먼저 논의해 주세요.
3. PR에는 무엇을, 왜 바꿨는지 간단히 적어 주세요.

## 꼭 지켜 주세요

### 1. 한국어·영어를 함께 고칩니다

이 문서는 한·영 병기입니다. `ko/`와 `en/`의 같은 파일을 **항상 한 쌍으로** 수정해 주세요. 한쪽만 바뀌면 두 언어 버전이 어긋납니다.

### 2. 한 일과 계획을 구분합니다

이 문서는 **이미 한 일의 기록**입니다. 계획이나 구상을 '했다'고 적으면 안 됩니다. 각 항목에는 상태 표시를 붙여 주세요.

| 표시 | 의미 |
|:----|:----|
| ✅ | 구현 완료 |
| 🔧 | 부분 구현 또는 개발 중 |
| ⬜ | 향후 과제 |
| 빠띠 오리지널 | 빠띠가 자체 개발한 고유 도구 |

확실하지 않으면 보수적으로 분류하고, PR 설명에 근거를 적어 주세요. 마크다운 표기는 다음과 같습니다.

```markdown
### N. 기능 이름

✅ 구현 완료
{: .label .label-green }
```

(`🔧`는 `.label .label-yellow`, `⬜`는 `.label`, 빠띠 오리지널은 `.label .label-purple`)

### 3. 항목 번호와 개수를 맞춥니다

- 카테고리 중간에 항목을 추가하면 **뒤 항목 번호가 모두 한 칸씩 밀립니다.** 같은 파일 안의 상호참조(`○○번 항목 참고`)도 함께 고쳐 주세요.
- 항목 수가 바뀌면 루트 `index.md`의 카테고리별 개수 표와 총계도 갱신해 주세요. 한·영 두 줄 모두입니다.

### 4. AI 관련 항목은 세 원칙을 따릅니다

빠띠는 민주적 의사결정에 관여하는 AI를 세 원칙으로 판단합니다 — **설명 가능성, 시민 참여형 합의, 중단할 권리**. AI 기능을 추가·수정할 때는 이 관점과 어긋나지 않게 써 주세요. 자세한 내용은 `11-ai-future.md`를 참고하세요.

## 저장소 구조

```
digital-democracy-100/
├── index.md                 # 메인 랜딩 페이지 (한·영 병기, 개수 표 포함)
├── ko/                      # 한국어 페이지 (index.md + 01~11)
├── en/                      # 영어 페이지 (index.md + 01~11)
├── _config.yml              # Jekyll & Just the Docs 설정
└── CONTRIBUTING.md
```

사이트는 Jekyll과 [Just the Docs](https://just-the-docs.com/) 테마로 빌드됩니다. 로컬에서 미리 보려면 `bundle exec jekyll serve`를 실행하세요.

## 행동 규약

이 저장소는 빠띠의 가치 위에서 운영됩니다. 서로를 존중하고, 다정하게 토론해 주세요. 모든 기여자는 [빠띠](https://parti.coop)가 지향하는 상냥하고 다정한 협력의 태도를 함께 지켜 주시기를 바랍니다.

## 라이선스

기여하신 내용은 이 저장소의 라이선스인 [크리에이티브 커먼즈 저작자표시 4.0 국제 라이선스(CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/deed.ko)를 따릅니다. 누구나 자유롭게 공유·활용·수정할 수 있으며, 출처(빠띠)를 표시하면 됩니다.

---

# Contributing

This is a **living document** that records the features and programs of digital democracy Parti has built. It is not a static catalog — new features are added as Parti builds them, and better descriptions are incorporated as they are suggested. Corrections, additions, and translations are welcome.

## What you can contribute

- **Corrections** — factual errors, typos, broken links.
- **Better descriptions** — clearer or more accurate wording.
- **Status updates** — when a feature's implementation status has changed (see status markers below).
- **New items** — Parti features or programs not yet recorded.
- **Translation improvements** — more natural Korean or English wording.

## How to contribute

1. Open a [GitHub Issue](https://github.com/parti-coop/digital-democracy-100/issues/new) to suggest a change, or send a Pull Request if you can make the fix yourself.
2. Small corrections can go straight to a PR without an Issue. For new items or larger structural changes, please open an Issue to discuss first.
3. In your PR, briefly note what you changed and why.

## Please follow these rules

### 1. Edit Korean and English together

This document is bilingual. Always edit the matching files in `ko/` and `en/` **as a pair**. Changing only one side leaves the two language versions out of sync.

### 2. Distinguish what is done from what is planned

This document is a **record of what has already been done**. Do not describe a plan or intention as something completed. Attach a status marker to every item.

| Marker | Meaning |
|:-------|:--------|
| ✅ | Implemented |
| 🔧 | In progress or partially implemented |
| ⬜ | Future direction |
| Parti Original | Independently developed by Parti |

When unsure, classify conservatively and explain your reasoning in the PR. The markdown is:

```markdown
### N. Feature Name

✅ Implemented
{: .label .label-green }
```

(`🔧` uses `.label .label-yellow`, `⬜` uses `.label`, Parti Original uses `.label .label-purple`.)

### 3. Keep item numbers and counts consistent

- Inserting an item mid-category **shifts every following item number by one.** Update in-file cross-references ("see item N") as well.
- When item counts change, update the per-category table and the total in the root `index.md` — both the English and Korean lines.

### 4. AI items follow the three principles

Parti judges AI involved in democratic decision-making by three principles — **explainability, citizen-participatory consensus, and the right to pause**. When adding or editing an AI feature, keep the wording consistent with this stance. See `11-ai-future.md` for details.

## Repository structure

```
digital-democracy-100/
├── index.md                 # Main landing page (bilingual, includes count table)
├── ko/                      # Korean pages (index.md + 01–11)
├── en/                      # English pages (index.md + 01–11)
├── _config.yml              # Jekyll & Just the Docs configuration
└── CONTRIBUTING.md
```

The site is built with Jekyll and the [Just the Docs](https://just-the-docs.com/) theme. To preview locally, run `bundle exec jekyll serve`.

## Code of conduct

This repository operates on Parti's values. Please be respectful and discuss with kindness. All contributors are asked to uphold the warm, considerate spirit of collaboration that [Parti](https://parti.coop) stands for.

## License

Your contributions are subject to this repository's license, [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). Anyone is free to share, adapt, and build upon the material, as long as appropriate credit is given to Parti.

---

*Made with 🇰🇷 by [Parti Cooperative](https://parti.coop).*
