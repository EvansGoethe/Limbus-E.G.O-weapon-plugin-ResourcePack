# Limbus E.G.O Weapons — Plugin ResourcePack

> Face the sin, Save the E.G.O.

搭配 [Limbus E.G.O Weapons](https://github.com/EvansGoethe/Limbus-E.G.O-Weapons) 插件（Paper）與 [Fabric mod](https://github.com/EvansGoethe/Limbus-E.G.O-Weapons) 使用的 Minecraft 資源包，內含 Limbus Company 中登場之 E.G.O 武器的 3D 模型、貼圖、與部分自訂音效。

- **遊戲版本**：Minecraft **1.21.4+**
- **pack_format**：`46`（支援範圍 `15 ~ 100`）
- **技術**：使用 1.21.4 的 `item-model` 元件（`assets/<namespace>/items/<id>.json`），已不再使用舊版 `custom_model_data`。

---

## 目錄結構

每把武器 / 彈藥各佔一個 namespace，統一放在 `assets/` 底下：

```
assets/
├── ringbrush/                  # 環指筆刷
├── mimicry/                    # 擬態
├── dacapo/                     # DaCapo
├── solemnlament/               # 莊嚴哀悼（黑 / 白）+ 生蝶亡蝶彈藥
├── shadow_vested_bladesinger/  # 著影揮刀
├── tiantui_star/               # 天退星刀 + 虎標彈 / 猛虎標彈
├── tibia/                      # 提比婭
├── twilight/                   # 薄暝 + 終末鳥
├── w_corp_knife/               # W 公司匕首
└── minecraft/                  # 覆寫 vanilla 資源（如 atlases、部分 items）
```

每個 namespace 下的標準子目錄：

```
<namespace>/
├── items/       # 1.21.4 item-model 定義
├── models/item/ # 3D 模型（.json，通常由 BlockBench 匯出）
├── textures/item/ # 貼圖（.png）
└── sounds/      # 自訂音效（僅部分武器）
```

---

## 收錄武器

| 中文名 | Namespace / ID | 底材 |
|---|---|---|
| 環指筆刷 | `ringbrush` | `NETHERITE_SWORD` |
| 擬態 | `mimicry` | `DIAMOND_SWORD` |
| DaCapo | `dacapo` | `IRON_SWORD` |
| 莊嚴哀悼（黑 / 白） | `solemnlament` | `CROSSBOW` |
| 生蝶亡蝶（莊嚴哀悼專用彈藥） | `solemnlament` | `ARROW` |
| 著影揮刀 | `shadow_vested_bladesinger` | `NETHERITE_SWORD` |
| 天退星刀 | `tiantui_star` | `NETHERITE_SWORD` |
| 虎標彈 / 猛虎標彈 | `tiantui_star` | `GUNPOWDER` |
| 提比婭 | `tibia` | — |
| 薄暝 | `twilight` | `DIAMOND_SWORD` |
| 終末鳥 | `twilight` | `TRIAL_KEY` |
| W 公司匕首 | `w_corp_knife` | — |

> 完整武器機制、指令與圖鑑請見 [Limbus E.G.O Weapons 插件本體](https://github.com/EvansGoethe/Limbus-E.G.O-Weapons)。

---

## 安裝方式

### 方法 1：由插件自動發送（推薦）

只要伺服器安裝了 `Limbus E.G.O Weapons` 插件，玩家進伺服器時會自動下載本資源包（或由外部 ResourcePackManager 合併分發）。**玩家端無須手動安裝**。

### 方法 2：手動安裝

1. 前往 [Releases](https://github.com/EvansGoethe/Limbus-E.G.O-weapon-plugin-ResourcePack/releases) 下載最新版 `.zip`。
2. 放入 `.minecraft/resourcepacks/`。
3. 在 Minecraft 內啟用即可。

### 方法 3：自行打包

從本 repo 直接下載原始檔（或 `git clone`）後，把 `assets/`、`pack.mcmeta`、`pack.png` **內容**（不含外層資料夾）壓成 `.zip` 即可使用。

---

## 版本 & 發布流程

- 每次新增 / 修改武器貼圖或模型後，於資源包 repo 建立新的 Release（例如 `v.2.17`），並上傳打包好的 `.zip`。
- 對應 Java 插件主類別中的 `PACK_URL` 與 `PACK_HASH` 需同步更新（SHA-1）。
- 詳細流程見開發者的工作流程指南。

---

## 授權 / 致謝

- 授權依 [LICENSE](LICENSE) 為準。
- 本資源包中的角色、武器名稱、原始設定等版權屬 **Project Moon / Limbus Company** 所有；本專案為非商業性同人資源包，僅供 Minecraft 玩家在自架伺服器內使用。
