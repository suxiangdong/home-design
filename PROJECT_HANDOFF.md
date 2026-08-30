# 自建别墅设计项目交接与迁移说明

更新日期：2026-08-30  
当前项目目录：`/Users/suxiangdong/code/home`  
用途：把当前设计依据、定稿文件、ImageGen 工作流和迁移步骤集中保存，便于换电脑后继续工作。

## 1. 当前状态

项目目前已经完成：

- 一层结构保留版平面图。
- 二层内退式阳台最终平面图。
- 前、后效果图。
- 前、后、左、右鸟瞰图。
- 近垂直俯瞰图。
- 七视图总览图。
- 后立面厨房后门、上下楼梯窗及后鸟瞰立面的一致性校准。
- 正面内退式阳台和左右侧一层顶部装饰横条的一致性校准。

项目已清理为约 23 MB 的精简成果包，只保留权威平面图、正式效果图、原始参考图、最终提示词和交接资料。

重要：本目录目前没有可依赖的 Git 历史，不能把 Git 当成迁移备份。应直接复制整个目录或制作压缩包。

## 2. 坐标与视图规则

- 平面图统一为上北、下南、左西、右东。
- 南侧是房屋正面，北侧是屋后。
- 后视图和后鸟瞰图均从北向南看，因此平面图东侧在后视画面中会出现在左边。
- 厨房位于东北侧。厨房后门位于厨房北墙的西端，也就是靠餐厅的内侧端。
- 从后视画面看，厨房后门位于偏左位置，但不能放在画面最左外角。

后续修改前必须先确认这套方向关系，避免再次把厨房后门或楼梯窗放反。

## 3. 当前权威文件

### 3.1 原始参考资料

原始附件已经从 macOS 临时目录归档到项目内，换电脑时必须一起复制：

| 文件 | 用途 |
| --- | --- |
| `references/source/original-front-effect.png` | 最初的正面建筑效果参考 |
| `references/source/original-rear-effect.png` | 屋后立面效果参考 |
| `references/source/original-first-floor-plan.png` | 用户提供的一层原始平面图 |

不要再依赖 `/var/folders/.../T/codex-clipboard-*.png`，这些系统临时文件可能随时被清理。

### 3.2 当前平面图

| 楼层 | 可编辑源文件 | 高清预览 | 状态 |
| --- | --- | --- | --- |
| 一层 | `output/floorplan/villa-first-floor-plan-structure-preserved.svg` | `output/floorplan/villa-first-floor-plan-structure-preserved.png` | 当前权威版本 |
| 二层 | `output/floorplan/villa-second-floor-plan-recessed-balcony.svg` | `output/floorplan/villa-second-floor-plan-recessed-balcony.png` | 当前权威版本 |

两张 PNG 均为 4200 x 2640。SVG 是继续修改平面图时的源文件，PNG 只作为检查和 ImageGen 参考。

为方便整套成果迁移，当前两层平面图的 PNG 与 SVG 副本也保存在 `output/imagegen/villa-views/final/floorplans/`。

旧平面方案已经清除，`output/floorplan/` 中目前只保留上述两套权威文件。

### 3.3 当前效果图

当前正式文件位于 `output/imagegen/villa-views/final/`：

| 文件 | 内容 | 尺寸 |
| --- | --- | --- |
| `00-contact-sheet.jpg` | 七视图总览 | 2160 x 1360 |
| `01-front-elevation.png` | 南侧正面效果图 | 1599 x 984 |
| `02-rear-elevation.png` | 北侧后效果图 | 1597 x 985 |
| `03-front-aerial.png` | 前鸟瞰图 | 1599 x 984 |
| `04-rear-aerial.png` | 后鸟瞰图 | 1599 x 984 |
| `05-left-aerial.png` | 西侧左鸟瞰图 | 1599 x 984 |
| `06-right-aerial.png` | 东侧右鸟瞰图 | 1599 x 984 |
| `07-top-down.png` | 北向朝上的近垂直俯瞰图 | 1134 x 1387 |

无版本后缀的文件始终代表当前正式版本。版本化候选图已经清除；当前正视图已体现家庭厅内退凹廊，左鸟瞰已补齐西侧连续装饰横条。

## 4. 最终建筑与空间要点

### 4.1 总体轮廓

- 两层现代住宅，宽体黑色四坡屋顶。
- 东西向外墙总长 17.00 m。
- 主体基准进深 10.15 m。
- 外墙参考厚度 280 mm，内墙参考厚度 240 mm。
- 一层入口墙向北内退约 0.70 m。
- 一层右侧主卧体块向南外突约 1.00 m。
- 二层不跟随右侧一层主卧外突。
- 右侧突出体屋面不可上人，不设置二楼小露台。
- 左侧卧室与客厅南墙保持齐平。

### 4.2 一层最终布局

一层原始结构关系保持不变，当前图纸主要优化展示、门窗表达和使用细节。

- A01：入户门廊，位于阳台下方雨棚范围。
- A02：玄关，增加鞋柜。
- A03/A04：客厅/大厅，与餐厅连续。
- A05：主卧 B，约 4.00 x 4.00 m。
- A05-1：开放式通长衣柜，采用左右更长、上下更窄的横向比例。
- A06：开放前厅，右侧保持开放，并设置通透屏风。
- A07：公卫/PS1，约 2.30 x 1.60 m，含淋浴。
- A08：次卧，约 4.00 x 3.55 m。
- A09：双跑楼梯间，每跑净宽参考约 1.00 m。
- A10：一层书房，约 2.52 x 3.55 m。取消书房的要求仅针对二层。
- A11：开放式餐厅。
- A12：厨房，约 4.42 x 3.24 m。
- A13：主卧 A，南向体块外突约 1.00 m。
- A14：衣帽间 A。
- A15：主卫/PS2，约 2.38 x 2.00 m。

一层使用约束：

- 厨房不设置北墙或东墙外窗，以便北墙和东墙连续布置橱柜。
- 厨房必须设置机械排烟与补风。
- 厨房后门开在北墙西端，靠餐厅一侧，不能开在东北外角。
- 主卧入口保留平开门；衣帽间和主卫使用墙内移门，避免门扇相互打架。
- 客厅南侧保留大窗。
- 卧室不在东墙或西墙开窗。
- 公卫窗向西，独立主卫窗向东。

### 4.3 二层最终布局

二层最终要求为 1 个主卧、3 个次卧、无书房，并保留家庭厅/过厅。

- B01：次卧 1，约 4.00 x 3.55 m。
- B02：楼梯间，与一层 A09 完全叠合。
- B03：家庭厅/过厅，包含会客区、阅读/茶歇区和媒体柜，避免空间空荡。
- B04：公卫/PS1，与一层 A07 湿区叠合。
- B05：开放前厅，右侧保持开放并设置通透屏风。
- B06：次卧 2，带开放式通长衣柜。
- B06-1：横向通长衣柜。
- B07：次卧 3，约 4.42 x 3.24 m。
- B08：主卧衣帽间。
- B09：主卫/PS2，与一层 A15 湿区叠合。
- B10：主卧套房，包含衣帽间和主卫。

二层开口约束：

- 家庭厅北侧只设置一个窗户。
- 家庭厅南侧采用四扇推拉玻璃门连接阳台。
- 卧室不在东墙或西墙开窗。
- 公卫窗向西，主卫窗向东。
- 楼梯后墙每层各一扇窄高窗，上下同轴。

### 4.4 排水与湿区

- PS1：二层 B04 公卫叠合一层 A07 公卫。
- PS2：二层 B09 主卫叠合一层 A15 主卫。
- PS1、PS2 沿湿区墙角集中设置。
- 污废水立管上下直通，尽量减少横支管。
- 施工前必须复核立管位置、降板范围、梁高和楼梯步数。

## 5. 阳台、屋檐与正面体块

- 二层家庭厅南墙相对主体南墙基准线内退 0.80 m。
- 阳台净深 1.60 m，由 0.80 m 墙体内退和 0.80 m 外挑组成。
- 主屋面水平挑檐 0.80 m。
- 檐口正投影与阳台栏杆外沿对齐。
- 0.80 m 挑檐可以覆盖阳台外挑的 0.80 m；墙体内退的 0.80 m 已位于主体屋面下方。
- 该结论为平面正投影计算。强风夹雨时阳台外沿仍可能进水。
- 檐沟、泛水、栏杆节点及悬挑结构必须由建筑和结构专业复核。
- 右侧一层主卧保持突出以增强层次，二层退回主体线，不能因此形成小露台。

较早的“家庭厅墙与左侧齐平”方案已经被后续的“家庭厅内退 0.80 m、形成有顶凹廊”方案取代。后续以当前二层平面图为准。

## 6. 立面与效果图一致性

### 6.1 统一风格

- 暖白或浅灰外墙，避免一层墙色与黑色装饰块过度重叠。
- 黑色门窗框、黑色竖向装饰带和黑色四坡屋顶。
- 温暖室内灯光，克制的庭院照明和现代低维护景观。
- 正面需保留入口内退、客厅体块层次、一层右主卧外突和二层内退阳台。

### 6.2 后立面当前基准

以后效果图 `02-rear-elevation.png` 为后立面开口的最高优先级基准。

二楼从后视画面左到右：

1. 左侧房间窗。
2. 独立黑色竖向装饰带。
3. 中部房间窗。
4. 白墙中的窄楼梯窗。
5. 独立黑色竖向装饰带。
6. 右侧房间窗。

一楼从后视画面左到右：

1. 厨房后门。
2. 餐厅窗。
3. 中部房间窗。
4. 黑色竖带内的一楼窄楼梯窗。
5. 右侧卧室窗。

`04-rear-aerial.png` 已按上述顺序校准。以后修改后鸟瞰图时，必须继续把 `02-rear-elevation.png` 作为开口与装饰带的权威参考。

## 7. ImageGen 工作流

### 7.1 当前生成环境

- 模型：`gpt-image-2`。
- 方式：Codex 自带 ImageGen CLI。
- 最终图常用参数：`--quality high --size 2048x1152`。
- 当前环境变量：`OPENAI_API_KEY`、`OPENAI_BASE_URL`。
- 环境变量当前写在 `~/.zshrc`，迁移时只重新配置变量，不能把真实密钥写进项目或本文档。
- 当前临时 Python 环境：`/private/tmp/codex-imagegen-venv`，不可迁移，换电脑后必须重建。

Codex ImageGen CLI 的可移植路径写法：

```bash
export CODEX_HOME="${CODEX_HOME:-$HOME/.codex}"
export IMAGE_GEN="$CODEX_HOME/skills/.system/imagegen/scripts/image_gen.py"
```

建议在新电脑创建独立虚拟环境：

```bash
python3 -m venv .venv-imagegen
source .venv-imagegen/bin/activate
python -m pip install --upgrade pip
python -m pip install openai pillow
```

在 `~/.zshrc` 重新设置：

```bash
export OPENAI_BASE_URL="你的服务地址"
export OPENAI_API_KEY="你的密钥"
```

不要把实际值提交到文档、Git、网盘公开链接或提示词文件。

### 7.2 提示词与局部编辑

- 最终提示词位于 `output/imagegen/villa-views/final/prompts/`。
- 当前后鸟瞰最终校准提示词：`04-rear-aerial-calibrate-to-rear-elevation.txt`。
- 当前后视图楼梯窗提示词：`02-rear-elevation-stair-window-correction.txt`。
- 当前正面阳台最终校准提示词：`01-front-elevation-recessed-balcony-correction-v2.txt`。
- 当前左鸟瞰横条校准提示词：`05-left-aerial-first-floor-cornice-correction.txt`。

清理后不再保留临时遮罩和定位图。后续需要局部编辑时，在 `tmp/imagegen/` 中重新生成当次遮罩与定位图；确认正式图后删除该临时目录。

局部编辑命令模板：

```bash
.venv-imagegen/bin/python "$IMAGE_GEN" edit \
  --model gpt-image-2 \
  --image output/imagegen/villa-views/final/需要修改的正式图.png \
  --image tmp/imagegen/当次定位图.png \
  --mask tmp/imagegen/当次遮罩.png \
  --prompt-file output/imagegen/villa-views/final/prompts/对应提示词.txt \
  --quality high \
  --size 2048x1152 \
  --out output/imagegen/villa-views/final/候选图-v2.png
```

遮罩编辑时，第一张输入图是编辑目标，遮罩只作用于第一张图；后续输入图是定位或设计参考。提示词中必须逐张说明输入图角色。换电脑后应先确认 `$IMAGE_GEN` 可用，也可以直接使用虚拟环境 Python 和 ImageGen 脚本的绝对路径。

### 7.3 版本管理规则

1. 不直接覆盖正式图，先输出新的 `-vN` 文件。
2. 逐张检查门窗、体块、屋顶、镜头、裁切和景观是否漂移。
3. 只在确认后把新版本复制到无后缀的正式文件。
4. 更新 `00-contact-sheet.jpg`。
5. 更新 `output/imagegen/villa-views/final/README.md` 和本交接文档。
6. 完成核对与校验后删除版本化候选图和 `tmp/` 临时资源，保持项目精简。

ImageGen 即使使用遮罩，也可能轻微改变镜头或未遮罩区域。后鸟瞰修正曾出现镜头变得过于正面的情况，因此必须人工检查完整画面，不能只检查被修改的局部。

## 8. 精简目录结构

- `PROJECT_HANDOFF.md`
- `TRANSFER_CHECKSUMS.sha256`
- `references/source/`：三张原始参考图。
- `output/floorplan/`：两层权威平面图的 SVG 与 PNG。
- `output/imagegen/villa-views/final/`：总览、七张正式效果图、最终提示词和迁移用平面图副本。

整个项目目录都属于迁移包。历史候选图、旧虚拟环境、早期渲染、檐口试验和临时遮罩已经清除，不再需要单独筛选。

## 9. 推荐迁移步骤

### 9.1 完整迁移

在当前电脑执行：

```bash
cd /Users/suxiangdong/code
tar -czf villa-home-2026-08-30.tar.gz home
```

将 `villa-home-2026-08-30.tar.gz` 复制到新电脑后解压。解压位置可以改变，项目内部全部使用相对路径。

### 9.2 新电脑恢复

1. 安装 Codex，并确认存在 ImageGen skill。
2. 解压项目目录。
3. 创建新的 Python 虚拟环境并安装 `openai`、`pillow`。
4. 在新电脑的 `~/.zshrc` 设置 `OPENAI_BASE_URL` 和 `OPENAI_API_KEY`。
5. 执行 `source ~/.zshrc`，或使用 `zsh -lic` 运行 ImageGen。
6. 打开两张当前平面图、后效果图、后鸟瞰图和总览图进行目视检查。
7. 使用校验清单确认文件传输完整。

### 9.3 校验命令

在项目根目录执行：

```bash
shasum -a 256 -c TRANSFER_CHECKSUMS.sha256
```

Linux 若没有 `shasum`，可使用：

```bash
sha256sum -c TRANSFER_CHECKSUMS.sha256
```

校验文件使用通用的两列 SHA-256 格式。

当前清单对应 2026-08-30 的精简项目快照，并排除了 `.DS_Store` 和清单文件自身。若迁移前继续修改了任何文件，应重新生成清单。

## 10. 后续工作注意事项

- 当前图纸属于方案设计与视觉表达，不能直接替代建筑、结构、给排水、电气、消防或施工图。
- 17.00 m x 10.15 m、墙厚、楼梯净宽和房间尺寸仍需现场测量及专业复核。
- 必须复核楼梯步数、平台、净高、梁位和楼梯窗标高。
- 必须复核阳台悬挑、栏杆、排水坡度、防水、泛水和檐沟。
- 必须复核厨房机械排烟、补风和后门开启范围。
- 必须复核公卫、主卫的立管、降板和洁具定位。
- 后续效果图修改的优先级：当前平面图 > 当前正/后效果图 > 当前鸟瞰图 > 原始参考图。
- 涉及后立面时，`02-rear-elevation.png` 是门窗和黑色装饰带的最高优先级参考。
- 涉及正面阳台时，`villa-second-floor-plan-recessed-balcony.svg` 是内退、外挑和檐口覆盖关系的最高优先级参考。

## 11. 快速核对清单

迁移后开始工作前，逐项确认：

- [ ] 三张原始参考图位于 `references/source/`。
- [ ] 一层当前 SVG/PNG 可以打开。
- [ ] 二层当前 SVG/PNG 可以打开。
- [ ] 七张正式效果图和总览图可以打开。
- [ ] 后效果图的一、二楼楼梯窗上下同轴。
- [ ] 后鸟瞰图的二楼楼梯窗在白墙中，右侧另有独立黑色竖带。
- [ ] 厨房后门位于后视图偏左、靠餐厅一端，而不是外角。
- [ ] 二层右侧没有小露台。
- [ ] 家庭厅南墙内退 0.80 m，阳台净深 1.60 m。
- [ ] `OPENAI_API_KEY` 和 `OPENAI_BASE_URL` 已在新电脑单独配置。
- [ ] `TRANSFER_CHECKSUMS.sha256` 校验通过。
