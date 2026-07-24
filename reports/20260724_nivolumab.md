---
generic_name: nivolumab
brand_names:
  - Opdivo
developers:
  - Ono Pharmaceutical
  - Medarex
  - Bristol Myers Squibb
targets:
  - PD-1
  - PDCD1
modality: monoclonal_antibody
antibody_format: fully_human_IgG4_kappa_S228P
therapeutic_areas:
  - oncology
  - immuno_oncology
diseases:
  - malignant melanoma
  - non-small cell lung cancer
  - renal cell carcinoma
first_approval_year: 2014
report_date: 2026-07-24
evidence_cutoff: 2026-07-24
status: published
---

# ニボルマブ（オプジーボ）

## まず3行で

- 悪性黒色腫をはじめ、多数の固形がんと一部の血液がんに使われる免疫チェックポイント阻害抗体である。
- 活性化T細胞上のPD-1に結合してPD-L1・PD-L2による抑制シグナルを遮り、患者自身の抗腫瘍T細胞を再活性化する。
- 腫瘍細胞を直接攻撃せず、がんが利用する免疫の「ブレーキ」を外す治療を実証し、PD-1阻害薬として世界で初めて承認された点が重要である。

## 1. どんな病気か

代表疾患として悪性黒色腫を取り上げる。メラニン産生細胞が悪性化する腫瘍で、皮膚の色や形が変化する病変として現れるほか、粘膜にも生じ得る。早期なら切除が中心だが、遠隔転移すると従来の細胞傷害性化学療法だけでは長期制御が難しかった。

黒色腫は遺伝子変異が多く、変異由来抗原をT細胞が異物として認識し得る。一方、抗原を認識して繰り返し刺激されたT細胞ではPD-1が増え、腫瘍細胞や腫瘍内免疫細胞が発現するPD-L1・PD-L2との結合により増殖、サイトカイン産生、細胞傷害が抑えられる。これは正常では炎症の暴走や自己免疫を防ぐ仕組みだが、腫瘍は免疫回避に利用する。[Iwaiら](https://doi.org/10.1073/pnas.192461099)

ただし、PD-1経路だけが免疫抵抗性を決めるわけではない。腫瘍抗原の乏しさ、抗原提示の欠損、T細胞が腫瘍へ入れない環境、別の抑制経路も関与するため、PD-L1発現を含め単一の指標だけでは奏効を完全に予測できない。[NCI](https://www.cancer.gov/types/skin/hp/melanoma-treatment-pdq)

## 2. なぜこの分子を標的にするのか

PD-1は主に活性化T細胞に発現する抑制性受容体である。抗原受容体からの刺激と同時にリガンドが結合すると、T細胞活性化シグナルを弱める。したがってPD-1を遮断すれば、特定の腫瘍抗原をすでに認識しているT細胞の反応を回復させられる。がん種ごとの単一ドライバーではなく、複数のがんが共有する免疫回避機構を標的にできることが長所である。

弱点も同じ生理機能に由来する。ブレーキ解除は腫瘍だけに限定されず、正常組織への免疫寛容を破って肺、腸管、肝臓、内分泌臓器などに炎症を起こし得る。また、反応には抗原提示と機能するT細胞が必要で、PD-1遮断だけでは免疫学的に「冷たい」腫瘍を必ずしも変えられない。

## 3. どんな抗体として設計されたか

### 開発企業

小野薬品はPD-1に関する研究基盤を持ち、2005年にMedarexと完全ヒト抗PD-1抗体の共同研究を開始した。Medarexのヒト抗体作製基盤を使って両社が候補を創製・開発し、2009年のMedarex買収後はBristol Myers Squibb（BMS）が権利を承継した。小野が日本を中心に、BMSがグローバル開発を進めた。[小野薬品](https://prd.ono-pharma.com/en/rd/licensing)

### 基本設計

ニボルマブは完全ヒトIgG4κ抗体で、PD-1の細胞外領域に結合し、PD-L1とPD-L2の双方を競合的に遮断する。PD-1陽性T細胞を殺すことが目的ではないため、強いADCC・CDCを持つIgG1ではなく、エフェクター機能が相対的に弱いIgG4が選ばれた。[Wangら](https://doi.org/10.1158/2326-6066.CIR-14-0040)

IgG4は生体内で半分子を交換し得るため、ヒンジ部のセリンをプロリンへ置換（S228P）して分子を安定化している。つまり「T細胞に結合し続けるが、そのT細胞は除去しにくい」という阻害抗体向けの設計である。日本の悪性黒色腫では、通常240 mgを2週ごと、または480 mgを4週ごとに点滴静注する。[PMDA添付文書](https://www.pmda.go.jp/PmdaSearch/iyakuDetail/180188_4291427A1024_1_74)

### 作用の仕組み

抗体がPD-1のリガンド結合を遮ると、腫瘍抗原特異的T細胞の増殖、活性化、細胞傷害が回復する。薬が腫瘍を直接溶解するのではなく、既存の免疫応答が最終的な実行役となる。このため一部では深く持続する反応が得られる一方、抗原認識やT細胞浸潤が不足する患者では反応しない。

## 4. 病態から作用まで

```mermaid
flowchart LR
    A["腫瘍抗原をT細胞が認識"] --> B["慢性刺激でT細胞にPD-1発現"]
    C["腫瘍・免疫細胞のPD-L1/PD-L2"] --> D["PD-1抑制シグナル"]
    B --> D
    D --> E["T細胞機能低下・免疫回避"]
    D -.->|ニボルマブがPD-1を遮断| G["増殖・細胞傷害活性を回復"]
    G --> H["免疫による腫瘍制御"]
```

## 5. 何が画期的だったのか

ニボルマブは2014年7月、日本で切除不能悪性黒色腫に承認され、世界初の承認PD-1阻害薬となった。[PMDA](https://www.pmda.go.jp/files/000209430.pdf)、[小野薬品](https://www.ono-pharma.com/sites/default/files/en/news/press/sm_cn140704.pdf) 進行黒色腫では、従来のダカルバジンと比べ生存と奏効を改善し、反応が長く続く患者がいることを示した。[Robertら](https://doi.org/10.1056/NEJMoa1412082) さらに、がん細胞固有の分子を一つずつ狙う発想から、複数がん種に共通する免疫制御を操作する発想へ治療軸を広げた。

> **一言で評価：** この抗体の革新性は、PD-1という生理的な免疫ブレーキを安全性に配慮したIgG4で遮断し、患者自身のT細胞を再び抗がん作用の主体にしたことにある。

## 6. 実際の医療での位置づけ

2026年7月24日時点の日本では、悪性黒色腫、非小細胞肺がん、腎細胞がん、胃がん、食道がんなど多数の適応がある。単剤のほか、イピリムマブ、化学療法、分子標的薬との併用に用いられ、がん種・病期・バイオマーカーで位置づけが異なる。

重要な副作用は免疫関連有害事象で、間質性肺疾患、大腸炎、肝障害、甲状腺・下垂体・副腎障害、1型糖尿病などがある。早期発見し、休薬・中止や副腎皮質ステロイドなどで過剰な免疫反応を抑える必要がある。自己免疫疾患、移植歴、臓器機能なども治療選択を難しくし得る。

## 7. 類薬との違い

| 項目 | ニボルマブ | ペムブロリズマブ | イピリムマブ |
|---|---|---|---|
| 標的 | PD-1 | PD-1 | CTLA-4 |
| 抗体形式 | 完全ヒトIgG4κ、S228P | ヒト化IgG4κ、S228P | 完全ヒトIgG1κ |
| 作用の場 | 主に末梢組織・腫瘍局所のT細胞 | 主に末梢組織・腫瘍局所のT細胞 | 主にT細胞活性化初期 |
| 設計上の特徴 | 低エフェクターIgG4 | 低エフェクターIgG4 | IgG1でCTLA-4を遮断 |
| 強み | 広い適応、併用選択肢 | 広い適応とバイオマーカー展開 | PD-1阻害と相補的 |
| 弱点 | 非奏効・免疫毒性 | 非奏効・免疫毒性 | 免疫毒性が強まりやすい |

ニボルマブとペムブロリズマブの基本思想は近い。より重要なのは、PD-1阻害とCTLA-4阻害が免疫応答の異なる段階を解放し、併用で効果を深め得る代わりに免疫毒性も増やす点である。

## 8. この抗体から学べること

- **疾患生物学：** がんの進行は腫瘍細胞の増殖だけでなく、免疫回避にも依存する。
- **標的選択：** 複数がん種が共有する宿主側の制御点は、腫瘍横断的な標的になり得る。
- **抗体設計：** 受容体を持つ有用なT細胞を残すため、Fcエフェクターを抑えたIgG4が適する。
- **残る課題：** 奏効予測、一次・獲得耐性、免疫毒性と併用強度の最適化は未解決である。
- **次に読む抗体：** イピリムマブ。T細胞活性化初期のCTLA-4遮断と比較すると理解がつながる。

## 参考文献

1. [オプジーボ点滴静注 添付文書（第28版）](https://www.pmda.go.jp/PmdaSearch/iyakuDetail/180188_4291427A1024_1_74), 医薬品医療機器総合機構（PMDA）, 2026（アクセス日：2026-07-24）
2. [Opdivo Initial Approval Review Report](https://www.pmda.go.jp/files/000209430.pdf), 医薬品医療機器総合機構（PMDA）, 2014（アクセス日：2026-07-24）
3. [Opdivo EPAR](https://www.ema.europa.eu/en/medicines/human/EPAR/opdivo), European Medicines Agency, 2026（アクセス日：2026-07-24）
4. [OPDIVO receives manufacturing and marketing approval in Japan](https://www.ono-pharma.com/sites/default/files/en/news/press/sm_cn140704.pdf), Ono Pharmaceutical, 2014（アクセス日：2026-07-24）
5. [Ono–Medarex collaborative research agreement](https://www.ono-pharma.com/sites/default/files/en/news/press/enews20050512.pdf), Ono Pharmaceutical / Medarex, 2005（アクセス日：2026-07-24）
6. [Involvement of PD-L1 on tumor cells in the escape from host immune system and tumor immunotherapy by PD-L1 blockade](https://doi.org/10.1073/pnas.192461099), Iwai Y et al., 2002
7. [In vitro characterization of the anti-PD-1 antibody nivolumab, BMS-936558, and in vivo toxicology in non-human primates](https://doi.org/10.1158/2326-6066.CIR-14-0040), Wang C et al., 2014
8. [Safety, activity, and immune correlates of anti-PD-1 antibody in cancer](https://doi.org/10.1056/NEJMoa1200690), Topalian SL et al., 2012
9. [Nivolumab in previously untreated melanoma without BRAF mutation](https://doi.org/10.1056/NEJMoa1412082), Robert C et al., 2015
10. [Melanoma Treatment (PDQ®)–Health Professional Version](https://www.cancer.gov/types/skin/hp/melanoma-treatment-pdq), National Cancer Institute, 2025（アクセス日：2026-07-24）
