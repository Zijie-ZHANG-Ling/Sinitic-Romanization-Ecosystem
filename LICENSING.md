# Licensing

# 授權說明

本 repository **Sinitic Romanization Ecosystem（漢語族語言／漢語方言羅馬字生態系統）**同時包含原創軟件代碼、羅馬字方案、mapping rules、結構化數據、字音表、文檔，以及部分第三方軟件組件和基於第三方語言資源產生的衍生數據。

由於不同內容具有不同的來源、性質及授權條件，本 repository 採用**分層授權（layered licensing）**方式。任何單一 license 均不應被理解為自動適用於 repository 中的所有文件及所有數據層。

This repository, **Sinitic Romanization Ecosystem**, contains original software code, romanization schemes, mapping rules, structured data, pronunciation dictionaries, documentation, as well as certain third-party software components and resources derived from third-party language data.

Because these materials have different origins, characteristics, and licensing conditions, this repository uses a **layered licensing model**. No single license should be interpreted as automatically applying to every file or every data layer contained in this repository.

---

## 1. Original Software Code

## 1. 原創軟件代碼

除非個別文件或目錄另有明確說明，本項目原創的軟件代碼以 **Apache License 2.0** 授權。

主要包括但不限於：

* **PhonEngine** 中由本項目自行開發的 PhonSymbol 及 PhonConvert 代碼；
* `convert_to_rime_yaml` 中由本項目自行開發的轉換工具；
* `cantromzj1_jyutping_py` 中由本項目自行開發的轉換、解析及處理代碼；
* 本 repository 中其他明確屬於本項目原創的軟件代碼。

本 repository 根目錄中的 `LICENSE` 文件載有 Apache License 2.0 的完整條款。

本項目的 Apache License 2.0 授權**不適用於 repository 中包含的第三方軟件組件**。相關第三方組件仍受其原始 license 約束。

Unless otherwise explicitly stated in an individual file or directory, original software code developed by this project is licensed under the **Apache License 2.0**.

This includes, but is not limited to:

* original PhonSymbol and PhonConvert code developed as part of **PhonEngine**;
* original conversion tools in `convert_to_rime_yaml`;
* original conversion, parsing, and processing code in `cantromzj1_jyutping_py`;
* other software code clearly identified as original work of this project.

The complete Apache License 2.0 text is provided in the root `LICENSE` file.

The Apache License 2.0 granted by this project **does not apply to third-party software components included in the repository**. Such components remain subject to their respective upstream licenses.

---

## 2. Original Romanization Schemes, Mapping Rules, and Project-Created Materials

## 2. 原創羅馬字方案、映射規則及本項目創作內容

除非個別文件或目錄另有明確說明，本項目有權授權的以下原創內容以 **Creative Commons Attribution 4.0 International（CC BY 4.0）** 授權：

* 本項目設計的 RomZJ 羅馬字方案；
* 本項目設計的 phoneme / phonological-unit → romanization mapping rules；
* tone mappings、tone representation rules 及其他 scheme-specific rules；
* 僅包含本項目原創方案結構、mapping 及相關說明的 PhonSymbol scheme JSON 文件；
* 本項目原創的 scheme-specific annotations、conversion rules 及 configuration；
* 本項目基於上述方案及 mapping rules 所創建的 RomZJ romanized representation layer；
* README、使用指南、方案設計說明及其他本項目原創文檔。

使用、修改或重新分發上述內容時，應按照 CC BY 4.0 的要求提供適當署名。

需要注意的是，**同一個 JSON、CSV 或其他數據文件中可能同時存在本項目原創內容與第三方來源內容**。CC BY 4.0 僅適用於本項目有權授權的原創部分，而不應被理解為自動重新授權同一文件中的第三方數據。

Unless otherwise explicitly stated, the following original materials that this project has the right to license are licensed under the **Creative Commons Attribution 4.0 International License (CC BY 4.0)**:

* RomZJ romanization schemes designed by this project;
* project-created phoneme / phonological-unit → romanization mapping rules;
* tone mappings, tone-representation rules, and other scheme-specific rules;
* PhonSymbol scheme JSON files containing project-created scheme structures, mappings, and related descriptions;
* original scheme-specific annotations, conversion rules, and configurations;
* the RomZJ romanized representation layer created by applying project-designed schemes and mapping rules;
* README files, usage guides, scheme-design documentation, and other original project documentation.

Appropriate attribution must be provided when these materials are used, modified, or redistributed in accordance with CC BY 4.0.

A single JSON, CSV, or other data file may contain both project-created content and third-party-derived content. The CC BY 4.0 license therefore applies only to original components that this project has the right to license and **should not be interpreted as automatically relicensing third-party data contained in the same file**.

---

## 3. Mixed-Source and Derived Resources

## 3. 混合來源及衍生資源

部分 PhonConvert editing-state JSON 文件及其生成的 CSV 字音表同時包含**本項目原創內容**與**第三方來源或第三方衍生數據**。

其中，本項目原創內容可能包括：

* RomZJ romanization scheme；
* mapping rules；
* tone mappings；
* scheme-specific annotations；
* conversion configuration；
* 由本項目方案生成的 romanized representations。

第三方來源或第三方衍生內容則可能包括：

* 漢字與字音之間的對應關係；
* 原始音系符號；
* 原始聲母、韻母、聲調或其他 pronunciation information；
* 多音字及不同 readings 之間的關係；
* 同音字 grouping；
* 字符收錄範圍；
* 由外部字音數據庫或 pronunciation resources 提供的其他信息。

即使第三方來源字音已被本項目的 romanization mapping 轉換為新的 RomZJ 表示，該轉換也不應被理解為自動消除、取代或重新授權底層第三方數據中原有的權利。

因此：

* 本項目創作的 **RomZJ schemes、mapping rules、annotations、conversion rules、configurations 及 romanized representation layer** 可按照適用的本項目 license 使用；
* 第三方來源或可由文件恢復、重構或推導出的底層字音信息仍受其原始來源的相關 copyright、license、terms of use 或其他適用條款約束；
* 本項目對原創 RomZJ layer 所提供的 license **不應被理解為對底層第三方 pronunciation data 的重新授權**；
* 若第三方來源本身具有開放 license，使用者亦可依照該 upstream license 對相應第三方內容行使權利。

Certain PhonConvert editing-state JSON files and the CSV pronunciation dictionaries generated from them contain both **original project-created contributions** and **third-party or third-party-derived data**.

Project-created components may include:

* RomZJ romanization schemes;
* mapping rules;
* tone mappings;
* scheme-specific annotations;
* conversion configurations;
* romanized representations generated using project-created schemes.

Third-party or third-party-derived components may include:

* character–pronunciation relationships;
* source phonological symbols;
* source initials, finals, tones, or other pronunciation information;
* relationships between polyphonic characters and their readings;
* homophone groupings;
* character coverage;
* other information originating from external pronunciation databases or language resources.

Even when third-party pronunciation information has been converted into a new RomZJ representation through project-created mapping rules, such transformation should not be interpreted as automatically removing, replacing, or relicensing rights associated with the underlying third-party data.

Accordingly:

* project-created **RomZJ schemes, mapping rules, annotations, conversion rules, configurations, and romanized representation layers** may be used under the applicable project licenses;
* underlying third-party pronunciation information, including information reconstructable or inferable from distributed files, remains subject to the applicable copyright, licenses, terms of use, and other conditions of its original source;
* licenses granted by this project for the original RomZJ layer **should not be interpreted as relicensing the underlying third-party pronunciation data**;
* where an upstream resource is itself openly licensed, users may separately exercise the rights granted by that upstream license with respect to the corresponding third-party content.

---

## 4. PhonEngine and Third-Party Software Components

## 4. PhonEngine 與第三方軟件組件

PhonEngine 主要由本項目自行開發的 **PhonSymbol** 及 **PhonConvert** 組成，其原創代碼按照本文件第 1 節所述，以 Apache License 2.0 授權。

PhonEngine 同時隨附部分並非由本項目開發的第三方 JavaScript libraries，目前包括：

* Babel；
* React；
* ReactDOM；
* Tailwind CSS。

這些第三方文件並不因被包含於 PhonEngine 中而成為本項目的原創代碼，也**不會因本項目採用 Apache License 2.0 而被重新授權為 Apache License 2.0**。

相關第三方組件仍受其各自的 upstream copyright notices 及 licenses 約束。具體來源及授權信息應參閱 PhonEngine 目錄中的 `THIRD_PARTY_NOTICES.md` 或其他相關說明文件。

PhonEngine primarily consists of **PhonSymbol** and **PhonConvert**, which were developed by this project. Original PhonEngine code is licensed under the Apache License 2.0 as described in Section 1.

PhonEngine also distributes certain third-party JavaScript libraries that were not developed by this project, currently including:

* Babel;
* React;
* ReactDOM;
* Tailwind CSS.

These third-party files do not become original project code merely because they are distributed with PhonEngine and **are not relicensed under the Apache License 2.0 used for original project software**.

They remain subject to their respective upstream copyright notices and licenses. Please refer to `THIRD_PARTY_NOTICES.md` or other relevant documentation within the PhonEngine directory for detailed source and licensing information.

---

## 5. RomZJ Pronunciation Resources

## 5. RomZJ 字音資源

RomZJ 各語言／方言方案的大規模字音資源通常由以下兩個主要數據層共同構成：

1. **第三方來源的 pronunciation-data layer**；
2. **本項目原創的 RomZJ romanization layer**。

其中，本項目原創的 RomZJ layer 包括 scheme design、mapping rules、conversion rules、scheme-specific annotations，以及利用這些規則生成的 romanized representations。

底層第三方 pronunciation-data layer 則按照其各自來源、copyright、license 及 terms of use 處理，**不因被轉換為 RomZJ representation 而由本項目重新授權**。

Large-scale pronunciation resources associated with the various RomZJ language and variety schemes generally consist of two principal data layers:

1. a **third-party pronunciation-data layer**; and
2. an **original project-created RomZJ romanization layer**.

The original RomZJ layer includes scheme design, mapping rules, conversion rules, scheme-specific annotations, and romanized representations generated through those rules.

The underlying third-party pronunciation-data layer remains subject to its respective source, copyright, license, and terms of use and **is not relicensed by this project merely because it has been converted into a RomZJ representation**.

### 5.1 CantRomZJ1

CantRomZJ1 的大規模字音資源，包括相關 PhonConvert editing-state JSON、CSV 字音表，以及 `cantromzj1_data/cantromzj1_table_from_lshk_jyutping_table` 中的相關數據，基於 **Linguistic Society of Hong Kong (LSHK) Jyutping Workgroup** 發布的 Jyutping 字音資料製作。

相關資源中：

* 底層漢字字音及 character–pronunciation relationships 來源於 LSHK Jyutping resources；
* CantRomZJ1 scheme、mapping rules、conversion logic 及 CantRomZJ1 romanized representations 為本項目的原創貢獻。

LSHK 的相關 Jyutping 字音數據本身以 **CC BY 4.0** 發布。該 upstream data 因此可由使用者按照 LSHK 所提供的 CC BY 4.0 license 使用。

本項目對 CantRomZJ1 原創 layer 所提供的 CC BY 4.0 授權，與 LSHK 對其原始 Jyutping 數據提供的 CC BY 4.0 授權屬於**來源不同但兼容的授權層**。本項目並不聲稱重新授權 LSHK 原始數據，而是對本項目自身創作的 CantRomZJ1 layer 提供授權。

相關資源在使用、修改或重新分發時，應同時保留對 LSHK Jyutping Workgroup 及本項目原創 CantRomZJ1 contribution 的適當 attribution。

Large-scale CantRomZJ1 pronunciation resources, including the relevant PhonConvert editing-state JSON files, CSV pronunciation dictionaries, and resources under `cantromzj1_data/cantromzj1_table_from_lshk_jyutping_table`, are based on Jyutping pronunciation data released by the **Jyutping Workgroup of the Linguistic Society of Hong Kong (LSHK)**.

Within these resources:

* underlying character pronunciations and character–pronunciation relationships originate from LSHK Jyutping resources;
* the CantRomZJ1 scheme, mapping rules, conversion logic, and CantRomZJ1 romanized representations are original contributions of this project.

The relevant LSHK Jyutping pronunciation data are themselves released under **CC BY 4.0**. Users may therefore exercise rights in that upstream data under the CC BY 4.0 license provided by LSHK.

The CC BY 4.0 license granted by this project for the original CantRomZJ1 layer and the CC BY 4.0 license granted by LSHK for the original Jyutping data are **compatible but distinct licensing layers originating from different contributors**. This project does not claim to relicense the original LSHK data; it licenses its own CantRomZJ1 contributions.

Appropriate attribution to both the LSHK Jyutping Workgroup and the original CantRomZJ1 contributions of this project should be retained when applicable.

### 5.2 MandRomZJ1

MandRomZJ1 的大規模字音資源由通過 **pypinyin** 獲得的普通話字音資料轉換而成。

相關 PhonConvert editing-state JSON 文件同時包含：

* 用於生成 MandRomZJ1 字音資源的 source pronunciation information；
* 本項目設計的 MandRomZJ1 scheme 及 mapping rules；
* conversion configuration；
* scheme-specific editing information。

由 editing state 生成的 CSV 字音表主要展示經 MandRomZJ1 mapping rules 轉換後得到的 romanized representations，但其中所保留的 character coverage、character–pronunciation relationships、多音字 readings 等底層信息仍來源於相關 upstream pronunciation data。

因此：

* **MandRomZJ1 scheme、mapping rules、conversion logic、annotations 及 MandRomZJ1 romanized representations 為本項目的原創 RomZJ layer，按照本項目適用的 CC BY 4.0 授權；**
* **底層 pypinyin / pinyin-data pronunciation data 不由本項目重新授權；**
* pypinyin、pinyin-data 及其相關 upstream resources 的 copyright、license、source notices 及 provenance requirements 應按照相應上游項目處理。

Large-scale MandRomZJ1 pronunciation resources are generated by converting Mandarin pronunciation information obtained through **pypinyin**.

The corresponding PhonConvert editing-state JSON files contain both:

* source pronunciation information used to generate MandRomZJ1 resources;
* the project-created MandRomZJ1 scheme and mapping rules;
* conversion configurations;
* scheme-specific editing information.

CSV pronunciation dictionaries generated from these editing states primarily contain romanized representations produced through MandRomZJ1 mapping rules. However, underlying information such as character coverage, character–pronunciation relationships, and polyphonic readings still originates from the relevant upstream pronunciation data.

Accordingly:

* **the MandRomZJ1 scheme, mapping rules, conversion logic, annotations, and MandRomZJ1 romanized representations constitute the original project-created RomZJ layer and are licensed under the applicable project CC BY 4.0 license;**
* **the underlying pypinyin / pinyin-data pronunciation data are not relicensed by this project;**
* copyright, licenses, source notices, and provenance requirements associated with pypinyin, pinyin-data, and their relevant upstream resources remain governed by those upstream projects.

### 5.3 Other RomZJ Schemes Based on the Multi-function Chinese Character Database

部分其他 RomZJ 羅馬字方案的大規模字音資源使用了**漢語多功能字庫（Multi-function Chinese Character Database）**中的字音資料。

目前包括部分用於：

* Meixian Hakka／梅縣客家話；
* Nanjing／南京話；
* Shanghai Wu／上海話；

等方案的資源。

本 repository **不包含漢語多功能字庫的完整數據庫，也不重新發布其原始網站本身**。

但是，部分 PhonConvert editing-state JSON 文件中保存了來源於漢語多功能字庫的字音信息。雖然這些信息並非以原數據庫的原始展示形式直接呈現，但相關 editing-state 文件可能保存足以恢復、重構或推導相應 source pronunciation records 的信息。

這些 editing-state JSON 同時包含本項目的：

* RomZJ romanization scheme；
* mapping rules；
* conversion configuration；
* scheme-specific annotations；
* 其他本項目原創 editing information。

由這些 editing-state 文件生成的 CSV 字音表不直接展示原始 pronunciation notation，而是展示按照本項目 RomZJ mapping rules 轉換後產生的 romanized representations。

因此：

* **本項目原創的 RomZJ schemes、mapping rules、conversion rules、annotations 及 romanized representations 按照本項目適用的 CC BY 4.0 授權；**
* **漢語多功能字庫來源的底層 pronunciation data 不由本項目重新授權；**
* editing-state JSON 或 CSV 中仍保留、反映、重構或衍生自第三方來源的 character coverage、character–pronunciation relationships、多音字 readings、同音字 grouping 等信息，仍可能受原始數據提供者的相關權利及條款約束；
* 除非日後取得原始數據提供者的明確授權或相關目錄另有說明，本項目對原創 RomZJ layer 提供的 CC BY 4.0 授權不應被解釋為對底層第三方字音數據提供 CC BY 4.0 授權。

Several large-scale pronunciation resources for other RomZJ schemes use pronunciation information originating from the **Multi-function Chinese Character Database**.

These currently include certain resources associated with:

* Meixian Hakka;
* Nanjing;
* Shanghai Wu;

and related schemes.

This repository **does not contain the complete Multi-function Chinese Character Database and does not reproduce the original database website itself**.

However, certain PhonConvert editing-state JSON files preserve pronunciation information originating from the Multi-function Chinese Character Database. Although this information is not presented in the same form as the original database interface, the editing-state files may contain sufficient information to restore, reconstruct, or infer corresponding source pronunciation records.

These editing-state JSON files also contain project-created:

* RomZJ romanization schemes;
* mapping rules;
* conversion configurations;
* scheme-specific annotations;
* other original editing information.

CSV pronunciation dictionaries generated from these editing states do not directly display the original pronunciation notation. Instead, they contain romanized representations generated through project-created RomZJ mapping rules.

Accordingly:

* **project-created RomZJ schemes, mapping rules, conversion rules, annotations, and romanized representations are licensed under the applicable project CC BY 4.0 license;**
* **the underlying pronunciation data originating from the Multi-function Chinese Character Database are not relicensed by this project;**
* information retained, reflected, reconstructed, or derived from third-party sources in editing-state JSON or CSV files—including character coverage, character–pronunciation relationships, polyphonic readings, and homophone groupings—may remain subject to the rights and terms of the original data provider;
* unless explicit permission from the original data provider is obtained in the future or a specific directory states otherwise, the CC BY 4.0 license applied to the original RomZJ layer should not be interpreted as granting CC BY 4.0 rights to the underlying third-party pronunciation data.

---

## 6. External Data Sources Supported by PhonConvert

## 6. PhonConvert 支持的外部數據來源

PhonConvert 可以接受及解析來自外部網站或數據源的資料，例如 **古音小鏡（Kaom.net）**。

本 repository 本身並不因 PhonConvert 支持這些輸入來源而包含、重新發布或重新授權相應外部網站的數據。

使用者自行從外部來源獲取並輸入 PhonConvert 的數據，仍受相關數據提供者的 copyright、license、terms of use 或其他適用條款約束。

PhonConvert can accept and parse data obtained from external websites or data sources, including **Kaom.net**.

Support for such an input source does not mean that this repository itself contains, redistributes, or relicenses data from the corresponding external website.

Data independently obtained by users from external sources and supplied to PhonConvert remain subject to the copyright, licenses, terms of use, and other applicable conditions of their respective providers.

---

## 7. External Software Dependencies

## 7. 外部軟件依賴

部分本項目原創軟件會調用第三方 Python packages 或其他外部軟件，例如 **PyCantonese**。

如果第三方軟件僅作為 dependency 使用，而其源代碼或數據並未被複製及重新分發於本 repository 中，則該 dependency 的存在並不意味着其源代碼或數據成為本 repository 的一部分。

本項目原創代碼仍按照本項目指定的 license 授權；第三方 dependencies 則繼續受其各自的 license 約束。

Some original software developed by this project depends on third-party Python packages or other external software, including **PyCantonese**.

Where third-party software is used only as a dependency and its source code or data are not copied and redistributed in this repository, the existence of that dependency does not make the third-party source code or data part of this repository.

Original project code remains licensed under the license specified by this project, while third-party dependencies remain subject to their respective licenses.

---

## 8. Rime-Compatible Outputs

## 8. Rime 兼容輸出

`convert_to_rime_yaml` 中的原創轉換程序由本項目自行開發，其軟件代碼按照本文件第 1 節以 Apache License 2.0 授權。

該工具可以將 pronunciation dictionaries 轉換為可由 **Rime** 輸入法使用的 YAML 文件。

需要注意的是，**輸出文件的數據授權取決於輸入數據本身的來源、數據層及授權條件**。將某個 pronunciation dictionary 轉換為 Rime-compatible YAML 並不會改變其底層第三方數據的 copyright 或 license。

其中，由本項目 RomZJ scheme 及 mapping rules 所產生的 romanized representation layer 仍按照本項目適用的 license 處理。

Original conversion software in `convert_to_rime_yaml` was developed by this project and is licensed under the Apache License 2.0 as described in Section 1.

The tool can convert pronunciation dictionaries into YAML files compatible with the **Rime** input-method ecosystem.

The licensing status of generated output data depends on the provenance, data layers, and licensing conditions of the input data. Converting a pronunciation dictionary into a Rime-compatible YAML representation does not alter the copyright or licensing status of underlying third-party data.

The romanized representation layer generated through project-created RomZJ schemes and mapping rules remains subject to the applicable project license.

---

## 9. Experimental File Lists and External Speech Datasets

## 9. 實驗文件列表與外部語音數據集

`sampled_file_names` 目錄記錄相關論文實驗中使用的部分外部語音數據集文件名稱，包括來自 **AISHELL-3** 及 **MDCC** 的 sample filenames。

本 repository **不包含或重新發布相關數據集中的音頻文件、轉錄文本或其他原始數據內容**。

這些文件名列表僅用於：

* 記錄實驗所使用的 samples；
* 提高實驗透明度；
* 幫助具有合法數據訪問權限的研究者重現相同的數據抽樣。

AISHELL-3、MDCC 及其他外部數據集仍受其各自的 license、data-use agreements、access conditions 及其他適用條款約束。

希望取得相關 audio、transcripts 或其他原始數據的使用者，應直接通過原始數據提供者依照其條款獲取。

The `sampled_file_names` directory records filenames of selected samples from external speech datasets used in the related experiments, including sample filenames from **AISHELL-3** and **MDCC**.

This repository **does not contain or redistribute the audio recordings, transcripts, or other original dataset content**.

These filename lists are provided only to:

* document the samples used in the experiments;
* improve experimental transparency;
* allow researchers who independently possess legitimate access to the corresponding datasets to reproduce the same sampling.

AISHELL-3, MDCC, and other external datasets remain subject to their respective licenses, data-use agreements, access conditions, and other applicable terms.

Users wishing to obtain the corresponding audio recordings, transcripts, or other original dataset materials should obtain them directly from the original data providers under the applicable terms.

---

## 10. Accompanying Paper and arXiv Preprint

## 10. 配套論文及 arXiv 預印本

本 repository 所對應的主要論文為：

**Zijie Zhang, Tan Lee, Yong Cao, and Benyou Wang.**
*Toward a Cross-Lingual Romanization Ecosystem for Sinitic Languages: A Paired Mandarin–Cantonese Case Study.*
Accepted at **ISCSLP 2026**.
**arXiv:2608.29170**
https://arxiv.org/abs/2608.29170

該 arXiv 預印本在提交時選擇的是 **arXiv.org Non-exclusive License to Distribute**：

https://arxiv.org/licenses/nonexclusive-distrib/1.0/

該授權表示提交者授予 **arXiv.org 永久、非獨占的論文分發權**。

需要特別說明的是：

* 該 arXiv 授權是**提交者授予 arXiv.org 的分發授權**；
* 它並不等同於 CC BY、CC BY-SA 或其他向一般公眾授予廣泛再利用或衍生作品權利的開放內容 license；
* 它不應被理解為允許第三方任意修改論文內容、製作衍生版本或將修改版本冒充為原作者版本；
* 本 repository 所使用的 Apache License 2.0 及 CC BY 4.0 **不自動適用於論文 PDF 或論文正文**；
* 論文的 copyright status 應按照適用的作者權利、arXiv submission terms，以及 ISCSLP / IEEE 最終出版協議處理。

除非另有明確聲明，repository 中對 software、schemes、mappings、data representations 及 documentation 所提供的 licenses **不構成對配套論文全文的重新授權**。

The principal paper accompanying this repository is:

**Zijie Zhang, Tan Lee, Yong Cao, and Benyou Wang.**
*Toward a Cross-Lingual Romanization Ecosystem for Sinitic Languages: A Paired Mandarin–Cantonese Case Study.*
Accepted at **ISCSLP 2026**.
**arXiv:2608.29170**
https://arxiv.org/abs/2608.29170

The arXiv preprint was submitted under the **arXiv.org Non-exclusive License to Distribute**:

https://arxiv.org/licenses/nonexclusive-distrib/1.0/

Under this submission license, the submitter grants **arXiv.org a perpetual, non-exclusive license to distribute the article**.

In particular:

* the arXiv license is a **distribution license granted by the submitter to arXiv.org**;
* it is not equivalent to CC BY, CC BY-SA, or another public-content license granting broad reuse or derivative-work permissions to the general public;
* it should not be interpreted as permission for third parties to arbitrarily modify the article, create derivative versions, or represent modified versions as the original authors' work;
* the Apache License 2.0 and CC BY 4.0 licenses used within this repository **do not automatically apply to the article PDF or article text**;
* copyright in the article remains subject to applicable author rights, the arXiv submission terms, and any final ISCSLP / IEEE publication agreement.

Unless explicitly stated otherwise, licenses granted in this repository for software, schemes, mappings, data representations, and documentation **do not constitute a relicensing of the full text of the accompanying paper**.

---

## 11. Suggested Citation

## 11. 建議引用格式

如在學術研究中使用本 repository、Sinitic Romanization Ecosystem、PhonEngine、CantRomZJ1、MandRomZJ1 或相關方法，建議引用配套論文。

目前可使用以下 arXiv citation：

```text
Zhang, Zijie, Tan Lee, Yong Cao, and Benyou Wang.
"Toward a Cross-Lingual Romanization Ecosystem for Sinitic Languages:
A Paired Mandarin–Cantonese Case Study."
arXiv preprint arXiv:2608.29170, 2026.
Accepted at ISCSLP 2026.
```

建議 BibTeX：

```bibtex
@article{zhang2026siniticromanization,
  title   = {Toward a Cross-Lingual Romanization Ecosystem for Sinitic Languages: A Paired Mandarin--Cantonese Case Study},
  author  = {Zhang, Zijie and Lee, Tan and Cao, Yong and Wang, Benyou},
  journal = {arXiv preprint arXiv:2608.29170},
  year    = {2026},
  note    = {Accepted at ISCSLP 2026}
}
```

正式 ISCSLP / IEEE bibliographic information、DOI、頁碼及出版信息在可用後將補充。

For academic research using this repository, the Sinitic Romanization Ecosystem, PhonEngine, CantRomZJ1, MandRomZJ1, or related methods, citation of the accompanying paper is recommended.

The following arXiv citation may currently be used:

```text
Zhang, Zijie, Tan Lee, Yong Cao, and Benyou Wang.
"Toward a Cross-Lingual Romanization Ecosystem for Sinitic Languages:
A Paired Mandarin–Cantonese Case Study."
arXiv preprint arXiv:2608.29170, 2026.
Accepted at ISCSLP 2026.
```

Suggested BibTeX:

```bibtex
@article{zhang2026siniticromanization,
  title   = {Toward a Cross-Lingual Romanization Ecosystem for Sinitic Languages: A Paired Mandarin--Cantonese Case Study},
  author  = {Zhang, Zijie and Lee, Tan and Cao, Yong and Wang, Benyou},
  journal = {arXiv preprint arXiv:2608.29170},
  year    = {2026},
  note    = {Accepted at ISCSLP 2026}
}
```

Formal ISCSLP / IEEE bibliographic information, DOI, page numbers, and publication details will be added when available.

---

## 12. Attribution

## 12. 署名

若使用本項目的原創 RomZJ schemes、PhonEngine、mapping rules、software、romanized representations、documentation 或其他資源，請按照相應 license 提供適當署名。

建議至少包含：

* **Sinitic Romanization Ecosystem**；
* 相關 scheme 或 software 名稱，例如 CantRomZJ1、MandRomZJ1 或 PhonEngine；
* 本 repository；
* 配套論文或 arXiv identifier `arXiv:2608.29170`。

若使用包含第三方來源或第三方衍生數據的資源，亦應按照相關 upstream licenses 及 terms 對原始數據提供者進行適當署名。

When using original RomZJ schemes, PhonEngine, mapping rules, software, romanized representations, documentation, or other project-created resources, please provide appropriate attribution as required by the applicable license.

Recommended attribution should include, where appropriate:

* **Sinitic Romanization Ecosystem**;
* the relevant scheme or software name, such as CantRomZJ1, MandRomZJ1, or PhonEngine;
* this repository;
* the accompanying paper or arXiv identifier `arXiv:2608.29170`.

When using resources containing third-party or third-party-derived data, appropriate attribution to the original data providers should also be provided as required by the corresponding upstream licenses and terms.

---

## 13. Folder-Specific Licensing and Provenance Information

## 13. 各目錄的具體授權與來源說明

由於本 repository 中不同語言方案及資源具有不同的數據來源，每個相關子目錄可以提供額外的：

* `LICENSE`;
* `NOTICE`;
* `THIRD_PARTY_NOTICES.md`;
* `README.md`;
* provenance / attribution documentation。

如某個特定文件或子目錄中的明確授權說明與本文件中的一般規則存在差異，則應以**與該文件或資源最直接相關的具體授權及來源說明**為準。

本文件不應被理解為擴大本項目對任何第三方內容的授權權利。

Because different language schemes and resources in this repository have different data sources, individual directories may provide additional:

* `LICENSE` files;
* `NOTICE` files;
* `THIRD_PARTY_NOTICES.md` files;
* `README.md` files;
* provenance and attribution documentation.

Where explicit licensing information associated with a specific file or directory differs from the general rules described here, the **more specific licensing and provenance information directly associated with that resource** takes precedence.

Nothing in this document should be interpreted as expanding this project's rights to license third-party content.

---

## 14. Contributions to the Ecosystem

## 14. 對本生態系統的貢獻

本項目旨在建立一個可由社區持續擴展的羅馬字生態系統。

未來 contributors 可以提交：

* 新語言或方言的 romanization schemes；
* 已有語言的 alternative schemes；
* PhonSymbol scheme files；
* PhonConvert editing-state files；
* pronunciation dictionaries；
* software tools；
* documentation；
* downstream integrations。

貢獻者應確保自己有權提交相關內容，並清楚標明任何第三方數據或軟件的來源及適用 license。

除非另有明確協議，向本 repository 提交貢獻即表示貢獻者同意其**原創貢獻部分**按照對應類型的 repository license 發布：

* software contributions → Apache License 2.0；
* original schemes, mappings, annotations, romanized representation layers, and documentation → CC BY 4.0。

任何第三方來源內容均不因被提交至本 repository 而被重新授權。

This project is intended to develop into a continuously extensible community-driven romanization ecosystem.

Future contributors may submit:

* romanization schemes for additional languages or varieties;
* alternative schemes for languages already represented;
* PhonSymbol scheme files;
* PhonConvert editing-state files;
* pronunciation dictionaries;
* software tools;
* documentation;
* downstream integrations.

Contributors should ensure that they have the right to contribute the submitted materials and should clearly identify the provenance and applicable licenses of any third-party data or software.

Unless otherwise explicitly agreed, submission of a contribution to this repository indicates that the contributor agrees to license the **original portion of their contribution** under the corresponding repository license:

* software contributions → Apache License 2.0;
* original schemes, mappings, annotations, romanized representation layers, and documentation → CC BY 4.0.

Third-party content is not relicensed merely because it is contributed to this repository.

---

## 15. Summary

## 15. 授權結構摘要

簡要而言，本 repository 的授權結構如下：

| 內容                                                           | 一般處理方式                                                                                          |
| ------------------------------------------------------------ | ----------------------------------------------------------------------------------------------- |
| 本項目原創軟件代碼                                                    | Apache License 2.0                                                                              |
| 本項目原創 RomZJ schemes / mappings / annotations / documentation | CC BY 4.0                                                                                       |
| 本項目原創 RomZJ romanized representation layer                   | CC BY 4.0                                                                                       |
| CantRomZJ1 底層 LSHK Jyutping 數據                               | LSHK upstream CC BY 4.0；不由本項目重新授權                                                               |
| CantRomZJ1 原創 scheme / mapping / RomZJ representation layer  | 本項目 CC BY 4.0                                                                                   |
| MandRomZJ1 底層 pypinyin / pinyin-data 字音數據                    | 遵循 upstream licenses / provenance；不由本項目重新授權                                                     |
| MandRomZJ1 原創 scheme / mapping / RomZJ representation layer  | 本項目 CC BY 4.0                                                                                   |
| 基於漢語多功能字庫的底層字音數據                                             | 不由本項目重新授權                                                                                       |
| 基於上述數據創建的原創 RomZJ scheme / mapping / representation layer    | 本項目 CC BY 4.0                                                                                   |
| PhonEngine 中的第三方 JavaScript libraries                        | 各自 upstream licenses                                                                            |
| PyCantonese 等 external dependencies                          | 各自 upstream licenses                                                                            |
| `convert_to_rime_yaml` 原創代碼                                  | Apache License 2.0                                                                              |
| Rime-compatible output data                                  | 原創 RomZJ layer 跟隨本項目 license；底層數據跟隨 upstream rights                                             |
| AISHELL-3 / MDCC sampled filenames                           | 實驗記錄用途；不重新發布原始 audio / transcripts                                                              |
| 配套論文及 arXiv PDF                                              | 不適用 repository 的 Apache / CC BY license；arXiv submission 採用 Non-exclusive License to Distribute |

In summary, the repository follows the general licensing structure below:

| Material                                                                                     | General treatment                                                                                                |
| -------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| Original project software code                                                               | Apache License 2.0                                                                                               |
| Original RomZJ schemes / mappings / annotations / documentation                              | CC BY 4.0                                                                                                        |
| Original project-created RomZJ romanized representation layer                                | CC BY 4.0                                                                                                        |
| Underlying LSHK Jyutping data used in CantRomZJ1 resources                                   | Upstream LSHK CC BY 4.0; not relicensed by this project                                                          |
| Original CantRomZJ1 scheme / mapping / RomZJ representation layer                            | Project CC BY 4.0                                                                                                |
| Underlying pypinyin / pinyin-data pronunciation data used in MandRomZJ1                      | Follow upstream licenses / provenance; not relicensed by this project                                            |
| Original MandRomZJ1 scheme / mapping / RomZJ representation layer                            | Project CC BY 4.0                                                                                                |
| Underlying pronunciation data originating from the Multi-function Chinese Character Database | Not relicensed by this project                                                                                   |
| Original RomZJ schemes / mappings / representation layers created from those resources       | Project CC BY 4.0                                                                                                |
| Third-party JavaScript libraries in PhonEngine                                               | Their respective upstream licenses                                                                               |
| External dependencies such as PyCantonese                                                    | Their respective upstream licenses                                                                               |
| Original `convert_to_rime_yaml` code                                                         | Apache License 2.0                                                                                               |
| Rime-compatible output data                                                                  | Original RomZJ layer follows project license; underlying data remain subject to upstream rights                  |
| AISHELL-3 / MDCC sampled filenames                                                           | Experimental documentation only; no original audio / transcripts redistributed                                   |
| Accompanying paper and arXiv PDF                                                             | Not covered by repository Apache / CC BY licenses; arXiv submission uses the Non-exclusive License to Distribute |

---

如對某個具體文件、字音表、software component 或數據來源的授權範圍存在疑問，請首先查閱相應目錄中的 README、NOTICE、LICENSE、THIRD_PARTY_NOTICES 或 provenance 說明。

If there is uncertainty regarding the licensing status of a specific file, pronunciation dictionary, software component, or data source, please first consult the README, NOTICE, LICENSE, THIRD_PARTY_NOTICES, or provenance documentation associated with the corresponding directory.
