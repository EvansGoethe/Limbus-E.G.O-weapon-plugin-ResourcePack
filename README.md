# Limbus E.G.O Weapons — Plugin ResourcePack

> Face the sin, Save the E.G.O.

[![Latest](https://img.shields.io/badge/latest-v.2.17-blue)](https://github.com/EvansGoethe/Limbus-E.G.O-weapon-plugin-ResourcePack/releases/latest)
[![MC](https://img.shields.io/badge/Minecraft-1.21.4%2B-green)](https://minecraft.net)
[![pack_format](https://img.shields.io/badge/pack__format-46-orange)]()

---

## 🌏 中文版

搭配 [Limbus E.G.O Weapons](https://github.com/EvansGoethe/Limbus-E.G.O-Weapons) 插件（Paper）與 Fabric mod 使用的 Minecraft 資源包，內含 Limbus Company 中登場之 E.G.O 武器的 **3D 模型、貼圖、與部分自訂音效**。

### 📦 最新版本：`v.2.17 — 提比婭 Tibia`

- **新增**：`assets/tibia/` — 配合插件 v2.6.6 的 **提比婭（Tibia）巨劍**（模型 / 貼圖 / `item-model`）
- **承前版本已含**：
  - `assets/shadow_vested_bladesinger/` — 著影揮刀
  - `assets/w_corp_knife/` — W 公司匕首
- **SHA-1**：`060302e85c12d23127b7c4eb3b7050c82615e20d`
- **下載**：[Limbus_E.G.O_Weapons_plugin_ResourcePack.v.2.17.zip](https://github.com/EvansGoethe/Limbus-E.G.O-weapon-plugin-ResourcePack/releases/download/v.2.17/Limbus_E.G.O_Weapons_plugin_ResourcePack.v.2.17.zip)

### 🔧 環境需求

| 項目 | 值 |
|---|---|
| 遊戲版本 | Minecraft **1.21.4+** |
| pack_format | `46`（支援範圍 `15 ~ 100`） |
| 模型元件 | 1.21.4 的 `item-model`（`assets/<namespace>/items/<id>.json`），**不再使用**舊版 `custom_model_data` |

### 📁 目錄結構

每把武器 / 彈藥各佔一個 namespace，全部放在 `assets/` 底下：

```
assets/
├── ringbrush/                  # 環指筆刷
├── mimicry/                    # 擬態
├── dacapo/                     # DaCapo
├── solemnlament/               # 莊嚴哀悼（黑 / 白）+ 生蝶亡蝶彈藥
├── shadow_vested_bladesinger/  # 著影揮刀
├── tiantui_star/               # 天退星刀 + 虎標彈 / 猛虎標彈
├── tibia/                      # 提比婭 ★ v.2.17 新增
├── twilight/                   # 薄暝 + 終末鳥
├── w_corp_knife/               # W 公司匕首
└── minecraft/                  # 覆寫 vanilla 資源（atlases 等）
```

每個 namespace 標準子目錄：`items/`（`item-model` 定義）、`models/item/`（3D 模型）、`textures/item/`（貼圖）、`sounds/`（自訂音效，僅部分武器）。

### ⚔️ 收錄武器一覽

| 中文名 | Namespace | 底材 |
|---|---|---|
| 環指筆刷 | `ringbrush` | `NETHERITE_SWORD` |
| 擬態 | `mimicry` | `DIAMOND_SWORD` |
| DaCapo | `dacapo` | `IRON_SWORD` |
| 莊嚴哀悼（黑 / 白） | `solemnlament` | `CROSSBOW` |
| 生蝶亡蝶（莊嚴哀悼彈藥） | `solemnlament` | `ARROW` |
| 著影揮刀 | `shadow_vested_bladesinger` | `NETHERITE_SWORD` |
| 天退星刀 | `tiantui_star` | `NETHERITE_SWORD` |
| 虎標彈 / 猛虎標彈 | `tiantui_star` | `GUNPOWDER` |
| **提比婭** ★ | `tibia` | — |
| 薄暝 | `twilight` | `DIAMOND_SWORD` |
| 終末鳥 | `twilight` | `TRIAL_KEY` |
| W 公司匕首 | `w_corp_knife` | — |

> 完整武器機制、指令與圖鑑請見 [Limbus E.G.O Weapons 插件本體](https://github.com/EvansGoethe/Limbus-E.G.O-Weapons)。

### 📥 安裝方式

**方法 1：由插件自動發送（推薦）** — 只要伺服器安裝了 Limbus E.G.O Weapons 插件，玩家進伺服器時會自動下載本資源包（或由外部 ResourcePackManager 合併分發），玩家端無須手動安裝。

**方法 2：手動安裝** — 前往 [Releases](https://github.com/EvansGoethe/Limbus-E.G.O-weapon-plugin-ResourcePack/releases) 下載最新版 `.zip`，放入 `.minecraft/resourcepacks/` 後在 Minecraft 內啟用。

**方法 3：自行打包** — `git clone` 本 repo 後，把 `assets/`、`pack.mcmeta`、`pack.png` **內容**（不含外層資料夾）壓成 `.zip` 即可。

### 🚀 版本 & 發布流程

- 每次新增 / 修改武器貼圖或模型後，在此 repo 建立新的 Release（例如 `v.2.17`），上傳打包好的 `.zip`。
- 對應 Java 插件主類別中的 `PACK_URL` 與 `PACK_HASH` 需同步更新（SHA-1）。

### 📜 授權 / 致謝

- 授權依 [LICENSE](LICENSE) 為準。
- 角色、武器名稱、原始設定等版權屬 **Project Moon / Limbus Company** 所有；本專案為非商業性同人資源包。

---

## 🌏 English

A Minecraft resource pack paired with the [Limbus E.G.O Weapons](https://github.com/EvansGoethe/Limbus-E.G.O-Weapons) Paper plugin (and companion Fabric mod). Ships **3D models, textures, and custom sounds** for the E.G.O weapons from *Limbus Company*.

### 📦 Latest release: `v.2.17 — Tibia`

- **Added**: `assets/tibia/` — the **Tibia** greatsword (model / textures / `item-model`), aligned with plugin v2.6.6.
- **Carried over from v.2.16**:
  - `assets/shadow_vested_bladesinger/` — Shadow-Vested Bladesinger
  - `assets/w_corp_knife/` — W Corp Knife
- **SHA-1**: `060302e85c12d23127b7c4eb3b7050c82615e20d`
- **Download**: [Limbus_E.G.O_Weapons_plugin_ResourcePack.v.2.17.zip](https://github.com/EvansGoethe/Limbus-E.G.O-weapon-plugin-ResourcePack/releases/download/v.2.17/Limbus_E.G.O_Weapons_plugin_ResourcePack.v.2.17.zip)

### 🔧 Requirements

| Field | Value |
|---|---|
| Minecraft | **1.21.4+** |
| pack_format | `46` (supports `15 ~ 100`) |
| Model system | 1.21.4 `item-model` component (`assets/<ns>/items/<id>.json`). Legacy `custom_model_data` is **not** used. |

### 📁 Layout

Each weapon / ammo owns its own namespace under `assets/`:

```
assets/
├── ringbrush/                  # Ring Brush
├── mimicry/                    # Mimicry
├── dacapo/                     # DaCapo
├── solemnlament/               # Solemn Lament (Black / White) + Butterfly ammo
├── shadow_vested_bladesinger/  # Shadow-Vested Bladesinger
├── tiantui_star/               # Tiantui Star Sword + Tiger-Mark rounds
├── tibia/                      # Tibia   ★ new in v.2.17
├── twilight/                   # Twilight + Apocalypse Bird
├── w_corp_knife/               # W Corp Knife
└── minecraft/                  # vanilla overrides (atlases, etc.)
```

Standard subfolders per namespace: `items/` (`item-model` defs), `models/item/` (3D models), `textures/item/` (PNGs), `sounds/` (only for some weapons).

### ⚔️ Weapon roster

| Name | Namespace | Base item |
|---|---|---|
| Ring Brush | `ringbrush` | `NETHERITE_SWORD` |
| Mimicry | `mimicry` | `DIAMOND_SWORD` |
| DaCapo | `dacapo` | `IRON_SWORD` |
| Solemn Lament (Black / White) | `solemnlament` | `CROSSBOW` |
| Butterflies (Solemn Lament ammo) | `solemnlament` | `ARROW` |
| Shadow-Vested Bladesinger | `shadow_vested_bladesinger` | `NETHERITE_SWORD` |
| Tiantui Star Sword | `tiantui_star` | `NETHERITE_SWORD` |
| Tiger-Mark / Savage Tiger-Mark | `tiantui_star` | `GUNPOWDER` |
| **Tibia** ★ | `tibia` | — |
| Twilight | `twilight` | `DIAMOND_SWORD` |
| Apocalypse Bird | `twilight` | `TRIAL_KEY` |
| W Corp Knife | `w_corp_knife` | — |

Weapon mechanics, commands, and the in-game catalog live in the [main plugin repo](https://github.com/EvansGoethe/Limbus-E.G.O-Weapons).

### 📥 Installation

**Option 1 — auto-served by the plugin (recommended).** The plugin (or an external ResourcePackManager) pushes the pack to every player on join. No client-side work needed.

**Option 2 — manual.** Grab the latest `.zip` from [Releases](https://github.com/EvansGoethe/Limbus-E.G.O-weapon-plugin-ResourcePack/releases), drop it into `.minecraft/resourcepacks/`, enable in-game.

**Option 3 — build it yourself.** `git clone` this repo, then zip the **contents** of `assets/`, `pack.mcmeta`, `pack.png` (without the outer folder) into a `.zip`.

### 🚀 Release workflow

- Each time textures / models change, cut a new Release (e.g. `v.2.17`) and upload the packed `.zip`.
- Update `PACK_URL` and `PACK_HASH` (SHA-1) in the plugin's main class to match.

### 📜 License / credits

- See [LICENSE](LICENSE).
- Characters, weapon names, and original designs are © **Project Moon / Limbus Company**. This is a non-commercial fan resource pack.
