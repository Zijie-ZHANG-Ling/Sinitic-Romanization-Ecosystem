<p align="center">
☯️　🥢　🌏　🎋　🪭 🐉　⇄　🔤　🔠　🔡
</p>

# ☯️ 漢語族語言（漢語方言）羅馬字生態系統 🎋<br>🌏 漢字文化圈－大陸東南亞語言聯盟羅馬字生態系統 🥢
# 🔤 Sinitic Romanization Ecosystem 🔡<br>🔠 Sinosphere–MSEA Romanization Ecosystem 📝

## 概述
## Overview

「**Sinitic Romanization Ecosystem 漢語族語言（漢語方言）羅馬字生態系統**」是隨 ISCSLP 2026 論文 *Toward a Cross-Lingual Romanization Ecosystem for Sinitic Languages: A Paired Mandarin–Cantonese Case Study* 一同推出的核心開源生態系統。

**Sinitic Romanization Ecosystem** is the core open-source ecosystem introduced alongside the ISCSLP 2026 paper *Toward a Cross-Lingual Romanization Ecosystem for Sinitic Languages: A Paired Mandarin–Cantonese Case Study*.

本生態系統最初以漢語族語言（漢語方言）的跨語言羅馬字設計、數據與工具為核心，但其架構並不限於漢語族。其設計理念、數據格式與基礎設施可進一步擴展至漢字文化圈以及大陸東南亞語言聯盟（Mainland Southeast Asia, MSEA）中的其他語言，例如 Sinitic（漢語）、Vietic（越芒語）、Koreanic（韓語／朝鮮語）、Tai（台語）等。從這一更廣泛的發展方向而言，本項目亦可被稱為「**Sinosphere–MSEA Romanization Ecosystem 漢字文化圈－大陸東南亞語言聯盟羅馬字生態系統**」。

The ecosystem was initially developed around cross-lingual romanization design, data, and tools for Sinitic languages, but its architecture is not restricted to Sinitic. Its design methodology, data formats, and infrastructure can be extended to other languages across the **Sinosphere** and the **Mainland Southeast Asia (MSEA) linguistic area**, including, for example, Sinitic, Vietic, Koreanic, and Tai languages. In this broader sense, the project may also be referred to as the **Sinosphere–MSEA Romanization Ecosystem**.

本生態系統旨在建立一個**開放、可擴展、由社區共同建設的羅馬字資源與基礎設施平台**，使研究者、語言社群及開發者能夠為不同語言與方言設計、錄入、存儲、分享和擴展羅馬字方案，以及建立與之配套的字音表（pronunciation dictionaries）、結構化數據與下游工具。

The ecosystem aims to provide an **open, extensible, and community-driven platform for romanization resources and infrastructure**, enabling researchers, language communities, and developers to design, enter, store, share, and extend romanization schemes for different languages and varieties, together with pronunciation dictionaries, structured datasets, and downstream tools.

羅馬字方案及相關數據的**設計、錄入、結構化存儲、文件格式、共享方式與貢獻規範**將在本 README 及相關文檔中詳細介紹。我們希望任何新的語言、方言或替代方案都能在共同的數據規範與工具基礎上加入本生態系統，而不需要重新建立一套彼此不兼容的基礎設施。

Detailed specifications for the **design, entry, structured storage, file formats, sharing, and contribution of romanization schemes and related data** are provided in this README and the accompanying documentation. Our goal is to allow new languages, varieties, and alternative schemes to join the ecosystem through shared data standards and reusable tools rather than requiring each project to build an isolated and incompatible infrastructure from scratch.


---

## 生態系統的主要組成
## Components of the Ecosystem

本生態系統目前主要由以下四個部分組成：

The ecosystem currently consists of four major components:

### 1. 羅馬字設計原則
### 1. Romanization Design Principles

本生態系統提出一套面向跨語言羅馬字設計的基本框架，包括以下四項主要原則：

1. **語音對應（Phonetic Correspondence）**：跨語言中語音相近或相同的音位，應盡可能使用相近或相同的羅馬字符號表示；
2. **歷史音位對應（Historical-Phonological Correspondence）**：具有歷史同源關係的形式，應盡可能在羅馬字拼寫中保留可感知的相似性；
3. **一音一符（One-Phoneme-One-Symbol）**：同一音位原則上應具有穩定一致的符號表示；
4. **僅使用基本拉丁字符（Basic Latin / ASCII-oriented Representation）**：盡量使用基本拉丁字母及數字，以提高輸入法、數據存儲、軟件處理及跨平台使用的便利性。

The ecosystem proposes a general framework for cross-lingual romanization design based on four major principles:

1. **Phonetic Correspondence**: phonetically similar or identical phonemes across languages should, where possible, be represented by similar or identical romanized symbols;
2. **Historical-Phonological Correspondence**: historically related and cognate forms should, where possible, preserve perceivable spelling similarity in their romanized representations;
3. **One-Phoneme-One-Symbol**: the same phoneme should in principle receive a stable and consistent symbolic representation;
4. **Basic Latin / ASCII-oriented Representation**: basic Latin letters and digits are preferred where possible to facilitate input methods, data storage, software processing, and cross-platform implementation.

對於聲調語言，本生態系統另提出**調值－調類雙軌設計（dual-track tone representation）**。其中：

- **調值**使用趙元任五度標記法（Chao five-level tone system）表示實際音高；
- **調類**則使用本工作提出的 **Hierarchical Tone-Category Notation (HTCN)**，以階層式符號編碼聲調的歷史來源及分化關係。

具體設計理念、不同原則之間的取捨及實例，請參閱論文。

For tonal languages, the ecosystem additionally introduces a **dual-track tone representation**:

- **Tone values** represent phonetic pitch realization using the **Chao five-level tone system**;
- **Tone categories** represent historical origins and subsequent splits using the **Hierarchical Tone-Category Notation (HTCN)** introduced in this work.

For detailed motivations, trade-offs among the design principles, and concrete examples, please refer to the accompanying paper.


### 2. 具體語言／方言羅馬字方案 🪭
### 2. Romanization Schemes 🖌️

基於上述設計原則，本生態系統已經包含多套具體的語言／方言羅馬字方案。

其中，論文詳細介紹並分析了：

- **MandRomZJ1** — 普通話／現代標準漢語
- **CantRomZJ1** — 廣州粵語／穗港澳粵語

Based on the design principles above, the ecosystem already contains a number of concrete romanization schemes for individual languages and varieties.

The accompanying paper provides detailed descriptions and analyses of:

- **MandRomZJ1** — Mandarin / Modern Standard Chinese
- **CantRomZJ1** — Cantonese / Guangzhou–Hong Kong–Macau Cantonese

此外，目前 repository 中還包括：

- **MeixianKejiaRomZJ1** — 梅縣客家話方案一
- **MeixianKejiaRomZJ2** — 梅縣客家話方案二
- **NanjingRomZJ1** — 南京江淮官話／南京話
- **ShanghaiWuRomZJ1** — 上海吳語／上海話

The repository additionally contains:

- **MeixianKejiaRomZJ1** — Meixian Hakka romanization, Scheme 1
- **MeixianKejiaRomZJ2** — Meixian Hakka romanization, Scheme 2
- **NanjingRomZJ1** — Nanjing Jianghuai Mandarin
- **ShanghaiWuRomZJ1** — Shanghai Wu Chinese

上述方案均可作為生態系統中的獨立方案存在。同一語言亦可同時存在多套不同設計取向的方案，例如目前的兩套梅縣客家話方案。這意味着本生態系統並不要求每一種語言只有唯一的「標準答案」，而是提供共同的數據結構與基礎設施，使不同方案能夠被存儲、比較、測試和進一步發展。

Each scheme can exist independently within the ecosystem, and multiple alternative schemes may coexist for the same language or variety, as illustrated by the two current Meixian Hakka schemes. The ecosystem therefore does not assume that every language must have a single uniquely correct romanization. Instead, it provides shared data structures and infrastructure through which alternative schemes can be stored, compared, evaluated, and further developed.

MandRomZJ1 與 CantRomZJ1 的詳細設計論述已收錄於論文。梅縣客家話、南京話及上海話方案的詳細設計說明將陸續補充至本 repository。

Detailed descriptions of MandRomZJ1 and CantRomZJ1 are available in the paper. Documentation of the Meixian Hakka, Nanjing, and Shanghai schemes will be progressively added to this repository.


### 3. PhonEngine：核心數據與工具基礎設施 🎋
### 3. PhonEngine: Core Data and Tooling Infrastructure 📜

**PhonEngine 是本生態系統最核心的基礎設施之一。**

它旨在為不同語言、方言及不同羅馬字方案提供統一的**方案錄入、結構化存儲、字音數據製作及數據交換流程**，主要由兩個軟件組成：

**PhonEngine is one of the core infrastructure components of the ecosystem.**

It provides a unified workflow for **scheme authoring, structured storage, pronunciation-data construction, and data exchange** across different languages, varieties, and romanization schemes. It currently consists of two major tools:


#### PhonSymbol

**PhonSymbol** 是羅馬字方案的統一錄入與結構化存儲工具。

其主要功能包括：

- 提供統一的羅馬字方案錄入介面；
- 支持不同類型的音節結構；
- 將方案中的聲母、介音、韻腹、韻尾、成音節鼻音、韻母及聲調等單位結構化；
- 定義本生態系統中 romanization scheme 的 JSON 文件格式；
- 支持方案 JSON 的導入、導出、繼續編輯與共享。

**PhonSymbol** is the unified authoring and structured-storage tool for romanization schemes.

Its major functions include:

- providing a common interface for entering romanization schemes;
- supporting different types of syllable and phonological structures;
- structuring units such as initials, medials, nuclei, codas, syllabic nasals, finals, and tones;
- defining the JSON representation used for romanization schemes within the ecosystem;
- supporting the import, export, continued editing, and sharing of scheme JSON files.


#### PhonConvert

**PhonConvert** 是從音系資料及羅馬字方案批量建立大規模字音表的工具。

其主要功能包括：

- 將已有的語言／方言音系與漢字讀音資料導入統一工作流程；
- 將原始音系符號映射至目標羅馬字符號；
- 批量生成大規模羅馬字字音表；
- 保存完整的 **editing state**，使字音表的製作過程可以恢復、檢查、修改及重現；
- 定義本生態系統中字音表及相關 JSON／CSV 數據的標準格式；
- 為進一步的 G2P、P2G、輸入法、NLP、Speech 及語言資源處理提供結構化數據。

**PhonConvert** is a tool for constructing large-scale pronunciation dictionaries from existing phonological resources and romanization schemes.

Its major functions include:

- importing existing phonological and Chinese-character pronunciation resources into a unified workflow;
- mapping source phonological symbols to target romanized symbols;
- generating large-scale romanized pronunciation dictionaries;
- preserving complete **editing states**, allowing the construction process to be restored, inspected, modified, and reproduced;
- defining standardized JSON/CSV representations for pronunciation dictionaries and related data within the ecosystem;
- producing structured resources for downstream G2P, P2G, input methods, NLP, speech technology, and language-resource processing.

Together, **PhonSymbol + PhonConvert** define the standard workflow through which romanization schemes and their associated pronunciation data are created, stored, exchanged, reproduced, and extended within the ecosystem.


### 4. 其他基礎設施與生態兼容
### 4. Additional Infrastructure and Interoperability

除 PhonEngine 外，本 repository 還提供一系列用於實際部署及與既有語言技術生態互操作的工具與數據。

主要包括：

- 將 PhonConvert 生成的羅馬字字音表轉換為 **Rime** 輸入法兼容 YAML 文件的工具；
- 與既有 **Jyutping** 資源及 **PyCantonese** 生態高度兼容的 CantRomZJ1 數據與轉換工具；
- Jyutping ↔ CantRomZJ1 雙向轉換及 CantRomZJ1 音節解析工具；
- **PySinRom**：將相關功能進一步封裝並通過 PyPI 發布的 Python package；
- 面向後續 G2P、P2G、輸入法、ASR、TTS 及其他語言技術任務的可重用數據與接口。

Beyond PhonEngine, the repository provides additional tools and resources for practical deployment and interoperability with existing language-technology ecosystems.

These currently include:

- tools for converting pronunciation dictionaries generated by PhonConvert into **Rime-compatible YAML** input-method files;
- CantRomZJ1 resources and conversion tools designed for strong compatibility with the existing **Jyutping** and **PyCantonese** ecosystems;
- bidirectional Jyutping ↔ CantRomZJ1 conversion and CantRomZJ1 syllable parsing;
- **PySinRom**, a Python package distributed through PyPI that packages relevant functionality for convenient reuse;
- reusable data and interfaces for downstream G2P, P2G, input methods, ASR, TTS, and other language-technology applications.


---

## 一個開放且可持續擴展的生態系統
## An Open and Extensible Ecosystem

本 repository 並不僅僅用於保存論文中已經完成的幾套羅馬字方案，而是希望成為一個可以持續發展的開放生態系統。

研究者、語言社群及開發者可以在共同的 PhonEngine 數據規範下：

- 為新的語言或方言建立羅馬字方案；
- 為已有語言提出替代方案；
- 建立、修訂或擴充字音表；
- 開發新的轉換工具及下游應用；
- fork、修改並提交新的資源；
- 共同擴展整個 ecosystem 所覆蓋的語言與功能。

This repository is intended not merely as storage for the romanization schemes presented in the accompanying paper, but as a continuously extensible open ecosystem.

Under the shared PhonEngine data specifications, researchers, language communities, and developers are invited to:

- develop romanization schemes for additional languages and varieties;
- propose alternative schemes for languages already represented;
- construct, revise, and extend pronunciation dictionaries;
- develop new conversion tools and downstream applications;
- fork, modify, and contribute new resources;
- collectively expand the linguistic coverage and functionality of the ecosystem.

Detailed contribution procedures, file specifications, and recommended repository structures are described below.
