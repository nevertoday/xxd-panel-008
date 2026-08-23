<p align="center">
  <img src="./assets/banner.svg" alt="XXD Panel 008 project banner" width="1200">
</p>

<div align="center">

# 🦁 XXD Panel 008

### Translate a real photograph into a bright, quiet, intelligent pastel impossible space

[![Codex Skill](https://img.shields.io/badge/Codex-Skill-000000?style=flat-square)](./SKILL.md)
[![Four Modes](https://img.shields.io/badge/Modes-4-d75d32?style=flat-square)](#four-outputs-one-spatial-poem)
[![Raster Output](https://img.shields.io/badge/Output-PNG-3c6f67?style=flat-square)](#boundaries-and-trust)

<a href="README.md">简体中文</a> · <strong>English</strong> · <a href="README.ja.md">日本語</a> · <a href="README.ko.md">한국어</a> · <a href="README.ar.md">العربية</a>

</div>

> ORTHOGRAPHIC ISOMETRIC · PLATFORMS / STAIRS / DOORS · SPATIAL PARADOX · DYNAMIC PASTELS · MATTE 3D

XXD Panel 008 is an image-generation Skill for Codex and compatible agents. It translates the photograph's recognisable identity, silhouette, pose, and relation into platforms, stairs, doorways, arches, bridges, passages, floating structures, and impossible connections.

Height, path, connection, occlusion, isolation, and repetition carry the narrative through clean orthographic isometric space. Each work uses two to four luminous pastel main colours and one vivid jump point, finished as immaculate smooth matte 3D with one small geometric editorial line.

## Why it exists

“Poetic isometric space” easily collapses into arbitrary stairs, stock levels, and pastel architecture unrelated to the photograph.

008 reverses that logic:

```text
lock source facts → assign identity and relation to geometry → narrate through height / path / connection / occlusion / isolation / repetition → lock orthographic isometric camera → choose two to four dynamic pastels and one jump point → finish as immaculate matte 3D
```

If an unrelated photograph could replace the source without materially changing spatial metaphor, route, height relation, anchor geometry, colour jump, or copy, the result is not 008.

## The 008 visual contract

- **Source-bound spatial metaphor:** at least three identity, pose, action, function, emotion, or relation cues enter one geometric system.
- **Geometry has a job:** every platform, stair, doorway, arch, bridge, passage, floating structure, and impossible link maps to source facts.
- **Spatial narrative:** height carries hierarchy or distance; paths carry action; bridges and passages carry relation; occlusion, isolation, and repetition carry emotion and rhythm.
- **Orthographic isometric:** the camera is clean and geometry readable, without photographic perspective, crowded cities, labyrinth overload, or stock levels.
- **Dynamic pastel:** two to four cream, sandstone, pink, violet, blue, cyan, or mint mains create analogous harmony and warm/cool contrast.
- **One colour jump:** the entire image has exactly one purer orange-red, magenta, blue-green, or bright-yellow point at a decisive place.
- **Immaculate matte 3D:** smooth solid geometry, soft even light, and slight ambient shadow; no grain, paper, film, frost, old print, PBR, or harsh reflection.
- **Small spatial annotation:** exactly one thin geometric line, with no year, date, number, volume, giant title, or silent English translation.

## Samples · Coming soon

The repository reserves [`assets/examples/`](assets/examples/) for future work. Only finished 008 artwork verified by the project owner will be added; no post or image from another style is used as a placeholder.

Future samples will demonstrate 008's adaptability. Their subjects, spatial devices, palette, copy, and canvas ratios will never become generation references or defaults.

## Four outputs, one spatial poem

The four modes support single or multiple selection. Reply with `1`, `1+3`, `1,2,4`, or `all`; the Skill deduplicates and runs them in menu order 1→4. Every mode is delivered independently in its own task directory—never as an overview—and `all` yields seven PNGs per source (one for each ordinary mode plus four wallpapers). Sizes may be labelled by mode in the same reply; unlabeled ordinary modes remain source-adaptive. Copy is shared across selected modes by default and may be overridden per mode.

| Mode | Sizing logic | Deliverable |
| --- | --- | --- |
| `top-bottom` | source-adaptive | complete source above, 008 pastel impossible space below; both panels retain the source size and split exactly 50/50 |
| `left-right` | source-adaptive | complete source left, 008 pastel impossible space right; both panels retain the source size and split exactly 50/50 |
| `design-only` | source-adaptive | transformed design only, with no visible source photo; retains source ratio and dimensions |
| `wallpaper-pack` | four device sizes | separate phone, iPad, desktop, and children's-watch PNGs |

Exact user pixels > explicit ratio or destination > source adaptation for ordinary modes. The original `008.md` used a 3:4 creative canvas, but that historical example is not a silent default in the current Skill.

Photography in paired modes stays truthful, with only restrained grading and necessary environmental extension. Design-only and wallpapers still use the photograph as evidence but do not show it.

### Wallpaper packs: linked or independent

Wallpaper mode has no silent size default. Choose the common preset—phone `1440×3200`, iPad `2048×2732`, desktop `3840×2160`, watch `1024×1024`—or give labelled custom sizes.

- **Linked pack (recommended):** generate and approve the iPad anchor first; every other device references the original photo plus that same anchor and is recomposed for its canvas.
- **Independent set:** every device references only the source photograph and may explore different spatial metaphors, routes, height relations, pastel groups, and jump points.

Linked never means cropped. All four files are separately generated, composed, and reviewed, with no iPad→phone→desktop→watch reference chain.

## Copy leaves the spatial afterimage

Before generation, choose automatic copy, custom copy, or text-free output. Name the target language or locale whenever copy is present.

Automatic copy derives one short resonant line from visible emotion, relation, action, spatial tension, or supported story. It uses only the target language by default; bilingual output appears only when explicitly requested.

008 never adds a year, date, number, volume, or archival label to automatic copy for atmosphere and never silently appends an English translation. Exact user copy remains verbatim.

Finished user wording stays verbatim. A direction or editable draft is refined only while preserving audience, purpose, mandatory words, tone, and implication.

Language follows the intended audience rather than the command language:

```text
target market or audience > requested output language > direction language; if none is explicit, ask before generation
```

A Japanese edition uses natural Japanese, a Korean-audience edition uses natural Korean and correct spacing, a UK edition uses British English, and Arabic defaults to natural Modern Standard Arabic with genuine right-to-left composition. The Skill never guesses nationality from appearance, clothing, scenery, or signs and never uses pseudo-foreign text.

## Code guarantees geometry; image generation creates the artwork

The image model creates source-bound spatial metaphor, orthographic isometric geometry, dynamic pastels, one colour jump, immaculate matte 3D, and one small geometric annotation. `scripts/compose_panel.py` only plans canvases, performs exact 50/50 raster composition, finalises dimensions, and audits results. It never fakes artwork with programmatic drawing.

```bash
python3 scripts/compose_panel.py --plan --layout top-bottom --source photo.png
python3 scripts/compose_panel.py --plan --layout left-right --size 2560x1440
python3 scripts/compose_panel.py --audit result.png --layout design-only --size 2048x2048
```

Exact top-bottom canvases need an even total height; left-right canvases need an even total width. Requested pixels are never silently changed.

## Get started

```bash
git clone https://github.com/nevertoday/xxd-panel-008.git
mkdir -p ~/.codex/skills
ln -s "$(pwd)/xxd-panel-008" ~/.codex/skills/xxd-panel-008
```

Claude Code users may link the same directory to `~/.claude/skills/xxd-panel-008`. Restart the agent session after installation.

```text
$xxd-panel-008
Turn this photograph into a left-right composition. Derive the copy from the image and write it in natural Korean.
```

You may invoke the Skill with only a photograph. It first asks for one or more modes in a numbered multiline menu, then for copy settings; wallpaper mode also asks for linked/independent continuity and device sizes.

Full specifications:

- [Skill workflow](SKILL.md)
- [Chinese full prompt](references/xxd-panel-008-prompt.zh-CN.md)
- [English full prompt](references/xxd-panel-008-prompt.en.md)
- [Original style brief](references/008-source.md)

## Boundaries and trust

- Each photograph stays within its own task and never borrows subjects, colours, copy, or composition from other inputs, old results, or samples.
- Every invocation creates a fresh task directory; even identical sources and parameters must generate anew.
- Deliverables are PNG bitmaps, never SVG, HTML, Canvas, or programmatic-drawing substitutes.
- The configured bitmap bridge emits sanitised status only and does not expose providers, endpoints, headers, credentials, prompts, or response bodies.
- Each selected ordinary mode returns one file; selected `wallpaper-pack` adds four separate wallpapers. `all` returns seven PNGs per source across four sibling mode directories, never a contact sheet or overview.

Local composition needs Python 3 and Pillow. The safe bitmap bridge uses Python 3.11+ `tomllib`. Image generation still requires a host agent with built-in raster generation or an already configured compatible raster route.

## Repository

```text
xxd-panel-008/
├── SKILL.md
├── README.md / README.en.md / README.ja.md / README.ko.md / README.ar.md
├── agents/openai.yaml
├── assets/
│   ├── banner.svg
│   └── examples/ (reserved for future local samples)
├── scripts/
│   ├── compose_panel.py
│   └── configured_imagegen.py
└── references/
    ├── xxd-panel-008-prompt.zh-CN.md
    ├── xxd-panel-008-prompt.en.md
    └── 008-source.md
```

## About XXD

XXD is the abbreviated brand name of Xiaoxiaodong. This project is created and maintained by [@xiaoxiaodong01](https://x.com/xiaoxiaodong01).

## Support and Membership

### In-depth Consultation · CNY 299/hour

One-to-one consultation for using the Skills is billed at CNY 299 per hour. Contact Xiaoxiaodong through the WeChat QR code below to book.

### Xiaoxiaodong Skills User Community · CNY 99 to join

A one-time CNY 99 fee joins the community for workflow sharing, work discussion, and peer support. It does not include hourly one-to-one consultation. Include “Skills User Community” in your WeChat message.

### Knowledge Planet + Member Prompt Library · CNY 699/year

[Knowledge Planet](https://wx.zsxq.com/group/15554814142882) and the [XXD Member Prompt Library](https://vip.xiaoxiaodong.ai/) are one membership: **one annual payment unlocks both, with no second purchase required.**

1. Subscribe through [Knowledge Planet](https://wx.zsxq.com/group/15554814142882), then contact Xiaoxiaodong on WeChat for a Prompt Library redemption code.
2. Subscribe through the [Member Prompt Library](https://vip.xiaoxiaodong.ai/), then contact Xiaoxiaodong on WeChat for a Knowledge Planet invitation.

<p align="center">
  <a href="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png"><img src="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png" alt="XXD paid community WeChat QR code" width="320"></a>
</p>

<div align="center">

**Reality keeps the memory; geometry turns it into an emotion you can walk through.**

</div>

---

<div align="center">
  <h2>☕ Support this open-source project</h2>
  <p>If this project saved you time, a Star, a share, or a coffee helps keep it moving.</p>
  <table>
    <tr>
      <td align="center" width="240">
        <a href="https://github.com/nevertoday/zhongguo-traditional-colors/blob/main/docs/images/buy-me-a-coffee-qr.png?raw=true"><img src="https://github.com/nevertoday/zhongguo-traditional-colors/blob/main/docs/images/buy-me-a-coffee-qr.png?raw=true" alt="Support Xiaoxiaodong through Buy Me a Coffee" width="180"></a><br>
        <strong>Buy me a coffee</strong><br>
        <sub>Scan or open the QR code to support Xiaoxiaodong</sub>
      </td>
    </tr>
  </table>
  <p><sub>Support is entirely optional and never changes access to this open-source project.</sub></p>
</div>
