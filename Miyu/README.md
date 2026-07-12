# Miyu — Codex Animated Pet

<p align="center">
  <img src="screenshots/miyu-idle.png" alt="Miyu idle pose" width="160">
</p>

Miyu is a cheerful chibi manga character with vivid pink twin tails, navy ribbons, purple eyes, and a sailor-style outfit. She is packaged as a Codex sprite v2 pet with nine standard animation states and sixteen clockwise look directions.

미유는 분홍빛 트윈테일과 남색 리본, 보라색 눈이 특징인 귀여운 일본 만화풍 캐릭터입니다. Codex sprite v2 규격의 아홉 가지 기본 애니메이션과 열여섯 방향 시선을 지원합니다.

## Highlights

- Codex sprite contract: v2
- Atlas: `1536 × 2288` WebP with transparency
- Cell size: `192 × 208`
- Layout: 8 columns × 11 rows
- Standard states: idle, drag right, drag left, wave, jump, failed, waiting, working, review
- Look loop: 16 directions in 22.5-degree steps
- Public QA: atlas validation, three-reviewer blind direction validation, and final visual QA

## Animation previews

| Idle | Drag right | Drag left |
| --- | --- | --- |
| ![Idle](previews/idle.gif) | ![Drag right](previews/running-right.gif) | ![Drag left](previews/running-left.gif) |

| Wave | Jump | Failed |
| --- | --- | --- |
| ![Wave](previews/waving.gif) | ![Jump](previews/jumping.gif) | ![Failed](previews/failed.gif) |

| Waiting for input | Working | Review |
| --- | --- | --- |
| ![Waiting](previews/waiting.gif) | ![Working](previews/running.gif) | ![Review](previews/review.gif) |

## Full sprite and look-direction previews

<details>
<summary>Open the complete 8 × 11 animation sheet</summary>

![Miyu animation sheet](screenshots/animation-sheet.png)

</details>

<details>
<summary>Open the neutral + 16-direction QA sheet</summary>

![Miyu look directions](screenshots/look-directions.png)

</details>

## Install

From the repository root on macOS or Linux:

```bash
mkdir -p "$HOME/.codex/pets/miyu"
cp "Miyu/pet.json" "$HOME/.codex/pets/miyu/pet.json"
cp "Miyu/spritesheet.webp" "$HOME/.codex/pets/miyu/spritesheet.webp"
```

Restart or refresh the Codex desktop app if Miyu does not appear immediately.

To uninstall:

```bash
rm -rf "$HOME/.codex/pets/miyu"
```

## Required package files

Only these files are required by Codex:

```text
Miyu/
├── pet.json
└── spritesheet.webp
```

The `previews`, `screenshots`, and `qa` folders are documentation and verification artifacts for repository visitors.

## Verification

The published package passed the following checks:

- `spriteVersionNumber: 2`
- WebP RGBA, `1536 × 2288`
- 8 columns × 11 rows
- Transparent RGB residue: 0 pixels
- Atlas errors and warnings: none
- All fourteen randomized horizontal/vertical blind comparison pairs passed by strict majority
- All sixteen labeled look directions passed final visual review
- Published `pet.json` and `spritesheet.webp` checksums are listed in [`SHA256SUMS`](SHA256SUMS)

See [`qa/validation.json`](qa/validation.json), [`qa/direction-blind-validation.json`](qa/direction-blind-validation.json), and [`qa/final-visual-qa.json`](qa/final-visual-qa.json) for the public QA summaries.

## License

The package uses two licenses:

- `pet.json`, this README, `SHA256SUMS`, and files in `qa/` are available under the [MIT License](../LICENSES/MIT.txt).
- `spritesheet.webp`, images in `screenshots/`, and animations in `previews/` are available under [CC BY 4.0](../LICENSES/CC-BY-4.0.md).

When sharing or adapting Miyu's visual assets, use this attribution where practical:

> Miyu Codex Pet by Ryu JaeHyun, licensed under CC BY 4.0.

See the repository's [license overview](../LICENSE.md) for details.
