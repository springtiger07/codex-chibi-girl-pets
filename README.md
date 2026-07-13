# Codex Pets

Community-ready custom animated pets for the Codex desktop app.

Each pet folder contains the two files required for installation—`pet.json` and `spritesheet.webp`—plus screenshots, animation previews, and public QA results.

## Available pets

| Pet | Description | Preview |
| --- | --- | --- |
| [Hina](Hina/) | Miyu's slightly aloof sister with a golden-blonde ponytail and a teal-and-cream sailor outfit. | <img src="Hina/screenshots/hina-idle.png" alt="Hina" width="96"> |
| [Miyu](Miyu/) | A cheerful, pink twin-tailed chibi manga girl with nine standard animations and sixteen look directions. | <img src="Miyu/screenshots/miyu-idle.png" alt="Miyu" width="96"> |

## Repository layout

```text
codex-pets/
├── README.md
├── Hina/
│   ├── README.md
│   ├── pet.json
│   ├── spritesheet.webp
│   ├── previews/
│   ├── qa/
│   └── screenshots/
└── Miyu/
    └── ...
```

Open a pet folder for installation instructions and full previews.

## 한국어 안내

Codex 데스크톱 앱에서 사용할 수 있는 커스텀 애니메이션 펫 모음입니다. 현재 자매 캐릭터 미유와 히나를 제공하며, 각 펫 폴더에는 설치 파일, 동작 GIF, 전체 스프라이트 시트 미리보기와 공개용 검증 결과가 포함되어 있습니다.

## License

This repository uses a split license so the reusable package files and the character artwork have clear terms:

- Configuration, documentation, QA data, and any source code are licensed under the [MIT License](LICENSES/MIT.txt).
- Character artwork and visual assets in each pet's `spritesheet.webp`, `previews/`, and `screenshots/` are licensed under [Creative Commons Attribution 4.0 International](LICENSES/CC-BY-4.0.md).

See [LICENSE.md](LICENSE.md) for the exact scope and attribution guidance.
