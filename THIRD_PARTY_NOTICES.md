# Third-Party Notices

# 第三方來源及授權說明

本文件列出 **Sinitic Romanization Ecosystem（漢語族語言／漢語方言羅馬字生態系統）**目前使用、包含、依賴、引用或基於其數據產生衍生資源的主要第三方軟件、語言資源及數據集。

本文件主要用於提供**來源（provenance）、署名（attribution）及授權邊界（licensing boundaries）**說明。

本文件本身**不對任何第三方內容授予新的 license**。第三方軟件、數據及其他資源仍受其原始 copyright、license、terms of use、data-use agreement 或其他適用條款約束。

有關本 repository 的整體分層授權方式，請參閱 [`LICENSING.md`](./LICENSING.md)。

This document identifies major third-party software, language resources, and datasets that are currently included in, used by, depended upon by, referenced by, or used as sources for derived resources in the **Sinitic Romanization Ecosystem**.

Its purpose is to document **provenance, attribution, and licensing boundaries**.

This document **does not grant any new license to third-party content**. Third-party software, data, and other resources remain subject to their respective copyright, licenses, terms of use, data-use agreements, and other applicable conditions.

For the repository-wide layered licensing model, see [`LICENSING.md`](./LICENSING.md).

---

## 1. Third-Party Software Distributed with PhonEngine

## 1. 隨 PhonEngine 分發的第三方軟件

PhonEngine 的 PhonSymbol 及 PhonConvert 為本項目自行開發的軟件，但為了提供可直接在瀏覽器中運行的前端界面，相關目錄中同時隨附部分第三方 JavaScript libraries。

目前包括：

* **Babel**
* **React**
* **ReactDOM**
* **Tailwind CSS**

上述第三方 JavaScript 文件並非由本項目開發。

它們目前位於 PhonEngine 相關目錄的 `libs` 文件夾中，並與 PhonEngine HTML 文件一同分發。

這些第三方 library files **不適用於本項目原創代碼所採用的 Apache License 2.0**，而繼續受各自 upstream projects 的原始 copyright notices 及 licenses 約束。

目前上述組件均以其 upstream **MIT License** 條款分發。使用或重新分發這些文件時，應保留相應 upstream copyright 及 license notices。

更詳細的 PhonEngine 第三方軟件說明應參閱：

`PhonEngine/THIRD_PARTY_NOTICES.md`

PhonSymbol and PhonConvert are original software developed by this project. However, in order to provide browser-based user interfaces, PhonEngine also distributes several third-party JavaScript libraries.

These currently include:

* **Babel**
* **React**
* **ReactDOM**
* **Tailwind CSS**

These JavaScript files were not developed by this project.

They are currently distributed within `libs` directories associated with the PhonEngine HTML applications.

These third-party library files **are not covered by the Apache License 2.0 applied to original project software** and remain subject to the copyright notices and licenses of their respective upstream projects.

The above components are currently distributed by their upstream projects under the **MIT License**. Applicable upstream copyright and license notices should be retained when these files are used or redistributed.

For more detailed information about third-party software distributed with PhonEngine, see:

`PhonEngine/THIRD_PARTY_NOTICES.md`

---

## 2. PyCantonese

## 2. PyCantonese

本項目部分 Cantonese / Jyutping interoperability tools 使用 **PyCantonese** 作為外部 Python dependency。

例如，`cantromzj1_jyutping_py` 中的部分功能旨在與 PyCantonese 的 Jyutping representation 及 syllable-parsing workflow 保持兼容。

本 repository **不直接包含或重新分發 PyCantonese 的源代碼或其數據資源**；使用時由使用者另外安裝 PyCantonese。

PyCantonese 仍受其 upstream project 所提供的 license 約束。目前 PyCantonese software 採用 **MIT License**。

本項目自行開發的 interoperability / conversion code 與 PyCantonese 本身為不同的 software components，各自按照相應 license 處理。

Certain Cantonese / Jyutping interoperability tools in this project use **PyCantonese** as an external Python dependency.

For example, functionality under `cantromzj1_jyutping_py` is designed to interoperate with PyCantonese-style Jyutping representations and syllable-parsing workflows.

This repository **does not directly include or redistribute PyCantonese source code or its data resources**. Users install PyCantonese separately when required.

PyCantonese remains subject to the license of its upstream project. The PyCantonese software is currently distributed under the **MIT License**.

Project-created interoperability and conversion code and PyCantonese itself are separate software components and remain subject to their respective licenses.

---

## 3. LSHK Jyutping Resources

## 3. 香港語言學學會粵拼資源

部分 CantRomZJ1 字音數據基於 **Linguistic Society of Hong Kong (LSHK) Jyutping Workgroup** 發布的 Jyutping 字音資源製作。

主要涉及：

* `cantromzj1_data/cantromzj1_table_from_lshk_jyutping_table`
* CantRomZJ1 的部分 PhonConvert editing-state data
* CantRomZJ1 的相關 CSV pronunciation / homophone-character tables

相關資源中，底層的 Chinese-character pronunciation information 及 character–pronunciation relationships 來源於 LSHK Jyutping resources。

本項目在上述資源的基礎上加入並生成：

* CantRomZJ1 romanization scheme；
* CantRomZJ1 mapping rules；
* Jyutping → CantRomZJ1 conversion；
* CantRomZJ1 romanized representations；
* 相關 interoperability resources。

LSHK Jyutping Workgroup 的相關原始字音資源以 **Creative Commons Attribution 4.0 International（CC BY 4.0）** 發布。

因此，在適用情況下使用或重新分發相關 CantRomZJ1 resources 時，應同時保留：

1. 對原始 **LSHK Jyutping Workgroup** 資源的 attribution；
2. 對本項目 **CantRomZJ1** 原創 romanization layer 的 attribution。

本項目不聲稱重新授權 LSHK 的原始數據；LSHK 原始數據的相關權利直接來自其 upstream CC BY 4.0 license。

Certain CantRomZJ1 pronunciation resources are based on Jyutping resources released by the **Jyutping Workgroup of the Linguistic Society of Hong Kong (LSHK)**.

Relevant resources include:

* `cantromzj1_data/cantromzj1_table_from_lshk_jyutping_table`
* certain CantRomZJ1 PhonConvert editing-state data
* related CantRomZJ1 CSV pronunciation / homophone-character tables

Within these resources, the underlying Chinese-character pronunciation information and character–pronunciation relationships originate from LSHK Jyutping resources.

On top of these resources, this project contributes and generates:

* the CantRomZJ1 romanization scheme;
* CantRomZJ1 mapping rules;
* Jyutping → CantRomZJ1 conversion;
* CantRomZJ1 romanized representations;
* related interoperability resources.

The relevant original pronunciation resources released by the LSHK Jyutping Workgroup are licensed under the **Creative Commons Attribution 4.0 International License (CC BY 4.0)**.

Where applicable, use or redistribution of the corresponding CantRomZJ1 resources should therefore preserve:

1. attribution to the original **LSHK Jyutping Workgroup** resources; and
2. attribution to the original **CantRomZJ1** romanization layer created by this project.

This project does not claim to relicense LSHK's original data. Rights to the original LSHK data arise directly from its upstream CC BY 4.0 license.

---

## 4. pypinyin and Mandarin Pronunciation Resources

## 4. pypinyin 及普通話字音資源

MandRomZJ1 的部分大規模字音資源由通過 **pypinyin** 獲得的普通話 pronunciation information 轉換而成。

相關資源包括：

* MandRomZJ1 PhonConvert editing-state JSON files；
* 由上述 editing states 生成的 MandRomZJ1 CSV pronunciation / homophone-character tables。

其中：

* MandRomZJ1 scheme、mapping rules、conversion rules 及 MandRomZJ1 representations 為本項目原創內容；
* 底層 Chinese-character pronunciation information 及 character–pronunciation relationships 來源於 pypinyin 及其相關 upstream pronunciation resources。

pypinyin software 本身為外部第三方 software，並受其 upstream license 約束。

pypinyin 所提供或使用的 pronunciation information 亦可能涉及其相關 upstream datasets，例如 pinyin-data 及其他來源。因此，在重新使用相關 MandRomZJ1 large-scale pronunciation resources 時，應保留相關 upstream provenance 及適用的 copyright / license notices。

本項目**不對底層 pypinyin / upstream pronunciation data 進行重新授權**。

Certain large-scale MandRomZJ1 pronunciation resources are generated from Mandarin pronunciation information obtained through **pypinyin**.

Relevant resources include:

* MandRomZJ1 PhonConvert editing-state JSON files;
* MandRomZJ1 CSV pronunciation / homophone-character tables generated from those editing states.

Within these resources:

* the MandRomZJ1 scheme, mapping rules, conversion rules, and MandRomZJ1 representations are original project-created materials;
* the underlying Chinese-character pronunciation information and character–pronunciation relationships originate from pypinyin and its relevant upstream pronunciation resources.

The pypinyin software itself is third-party software and remains subject to its upstream license.

Pronunciation information provided through or used by pypinyin may also involve associated upstream datasets, including pinyin-data and other sources. Relevant upstream provenance and applicable copyright / license notices should therefore be retained when corresponding large-scale MandRomZJ1 pronunciation resources are reused.

This project **does not relicense the underlying pypinyin / upstream pronunciation data**.

---

## 5. Multi-function Chinese Character Database

## 5. 漢語多功能字庫

部分 RomZJ schemes 的大規模字音資源使用了**漢語多功能字庫（Multi-function Chinese Character Database）**中的 pronunciation information。

目前主要涉及部分：

* Meixian Hakka / 梅縣客家話；
* Nanjing / 南京話；
* Shanghai Wu / 上海話；

等 RomZJ resources。

相關 PhonConvert editing-state JSON files 中可能保存來源於漢語多功能字庫的：

* Chinese-character pronunciation information；
* source phonological information；
* character–pronunciation relationships；
* polyphonic readings；
* homophone relationships；
* 其他與字音相關的信息。

雖然相關信息並非以原數據庫網站的原始形式直接展示，但部分 editing-state files 可能包含足以恢復、重構或推導相應 source pronunciation records 的信息。

由相關 editing states 生成的 CSV pronunciation dictionaries 則包含經本項目 RomZJ mapping rules 轉換後的 romanized representations。

本項目原創的：

* RomZJ schemes；
* mapping rules；
* conversion rules；
* scheme-specific annotations；
* romanized representation layer；

按照本項目相應的 license 處理。

但是，來源於漢語多功能字庫的底層 pronunciation data **不由本項目重新授權**。

本 repository 不聲稱其 Apache License 2.0 或 CC BY 4.0 license 適用於上述第三方底層字音數據。

Certain large-scale pronunciation resources for RomZJ schemes use pronunciation information originating from the **Multi-function Chinese Character Database**.

These currently include certain resources associated with:

* Meixian Hakka;
* Nanjing;
* Shanghai Wu;

and related RomZJ schemes.

Relevant PhonConvert editing-state JSON files may preserve third-party information including:

* Chinese-character pronunciation information;
* source phonological information;
* character–pronunciation relationships;
* polyphonic readings;
* homophone relationships;
* other pronunciation-related information.

Although such information is not necessarily presented in the same form as the original database website, certain editing-state files may contain sufficient information to restore, reconstruct, or infer corresponding source pronunciation records.

CSV pronunciation dictionaries generated from these editing states contain romanized representations generated using project-created RomZJ mapping rules.

Original project-created:

* RomZJ schemes;
* mapping rules;
* conversion rules;
* scheme-specific annotations;
* romanized representation layers;

remain subject to the applicable project licenses.

However, the underlying pronunciation data originating from the Multi-function Chinese Character Database **are not relicensed by this project**.

This repository does not claim that its Apache License 2.0 or CC BY 4.0 license applies to such underlying third-party pronunciation data.

---

## 6. Kaom.net

## 6. 古音小鏡 Kaom.net

**PhonConvert** 支持將 **Kaom.net（古音小鏡）**作為外部 pronunciation / phonological data input source之一。

PhonConvert 可以解析由使用者提供的相關網頁內容，並將其轉換至統一的 phonology-and-romanization workflow。

但是：

* 本 repository **不包含 Kaom.net 的完整數據庫**；
* 本 repository **不因 PhonConvert 支持 Kaom.net 而重新發布或重新授權 Kaom.net 的數據**；
* 使用者自行從 Kaom.net 或其他外部來源取得的數據，仍受原始數據提供者的相關權利及使用條款約束。

**PhonConvert** supports **Kaom.net** as one possible external source of pronunciation and phonological data.

PhonConvert can parse relevant content supplied by users and transform it into the common phonology-and-romanization workflow.

However:

* this repository **does not contain the complete Kaom.net database**;
* support for Kaom.net does **not constitute redistribution or relicensing of Kaom.net data**;
* data independently obtained by users from Kaom.net or other external sources remain subject to the applicable rights and terms of the original providers.

---

## 7. AISHELL-3

## 7. AISHELL-3

部分 speech-to-romanization 實驗使用了 **AISHELL-3** speech dataset。

本 repository 的 `sampled_file_names` 目錄僅提供論文實驗中使用的部分 AISHELL-3 **sample filenames**，用於記錄實驗數據抽樣並提高 reproducibility。

本 repository：

* 不包含 AISHELL-3 audio recordings；
* 不包含 AISHELL-3 transcripts；
* 不重新發布 AISHELL-3 dataset 本身。

AISHELL-3 的原始數據仍受其 upstream dataset license 及相關條款約束。

The **AISHELL-3** speech dataset is used in certain speech-to-romanization experiments.

The `sampled_file_names` directory in this repository contains only selected AISHELL-3 **sample filenames** used in the experiments, for the purpose of documenting data sampling and improving reproducibility.

This repository:

* does not contain AISHELL-3 audio recordings;
* does not contain AISHELL-3 transcripts;
* does not redistribute the AISHELL-3 dataset itself.

Original AISHELL-3 data remain subject to the license and terms provided by the upstream dataset provider.

---

## 8. MDCC

## 8. MDCC

部分 Cantonese speech-to-romanization 實驗使用了 **MDCC** speech dataset。

本 repository 的 `sampled_file_names` 目錄僅記錄實驗中使用的部分 MDCC **sample filenames**。

本 repository：

* 不包含 MDCC audio recordings；
* 不包含 MDCC transcripts；
* 不重新發布 MDCC dataset 本身；
* 不因公開 sample filenames 而重新授權 MDCC 中的任何原始數據。

原始 MDCC data 仍受其 dataset provider 所規定的 license、data-use agreement、access conditions 及其他相關條款約束。

Certain Cantonese speech-to-romanization experiments use the **MDCC** speech dataset.

The `sampled_file_names` directory records only selected MDCC **sample filenames** used in those experiments.

This repository:

* does not contain MDCC audio recordings;
* does not contain MDCC transcripts;
* does not redistribute the MDCC dataset itself;
* does not relicense any original MDCC data by publishing sample filenames.

Original MDCC data remain subject to the license, data-use agreement, access conditions, and other applicable terms specified by the dataset provider.

---

## 9. Rime

## 9. Rime 輸入法生態

本項目提供由本項目自行開發的工具，用於將 PhonConvert pronunciation-dictionary outputs 轉換為 **Rime-compatible YAML** files。

本 repository 中的相關 converter code 為本項目原創軟件。

本項目提供 Rime-compatible output **並不表示本 repository 包含或重新發布 Rime 的源代碼**。

Rime software 本身仍受其 upstream project 的相應 license 約束。

輸出的 YAML data 則繼續受其輸入 pronunciation resource 的相關 licensing layers 約束。

This project provides original conversion tools for transforming PhonConvert pronunciation-dictionary outputs into **Rime-compatible YAML** files.

The relevant converter code in this repository is original project software.

Providing Rime-compatible output **does not mean that this repository contains or redistributes Rime source code**.

Rime software itself remains subject to the applicable license of its upstream project.

Generated YAML data remain subject to the licensing layers applicable to the input pronunciation resources.

---

## 10. Summary

## 10. 摘要

| 第三方來源                                      | 在本項目中的關係                                    | 是否直接分發第三方原始或衍生內容                                    |
| ------------------------------------------ | ------------------------------------------- | --------------------------------------------------- |
| Babel                                      | PhonEngine bundled JavaScript library       | 是，直接分發第三方 library files                             |
| React                                      | PhonEngine bundled JavaScript library       | 是，直接分發第三方 library files                             |
| ReactDOM                                   | PhonEngine bundled JavaScript library       | 是，直接分發第三方 library files                             |
| Tailwind CSS                               | PhonEngine bundled JavaScript library       | 是，直接分發第三方 library files                             |
| PyCantonese                                | External software dependency                | 否                                                   |
| LSHK Jyutping resources                    | CantRomZJ1 pronunciation-data source        | **是，repository 中包含部分來源內容及基於其產生的衍生內容**               |
| pypinyin / related pronunciation resources | MandRomZJ1 pronunciation-data source        | **是，editing-state / outputs 中包含部分來源信息及基於其產生的衍生內容**  |
| Multi-function Chinese Character Database  | 多個 RomZJ pronunciation-data source          | **是，editing-state /  outputs 中包含部分來源信息及基於其產生的衍生內容** |
| Kaom.net                                   | PhonConvert supported external input source | 否                                                   |
| AISHELL-3                                  | Experimental speech dataset                 | 否，僅提供 filenames                                     |
| MDCC                                       | Experimental speech dataset                 | 否，僅提供 filenames                                     |
| Rime                                       | Output interoperability target              | 否                                                   |

| Third-party source                         | Relationship to this project                        | Third-party source or derived content distributed in this repository?                                       |
| ------------------------------------------ | --------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| Babel                                      | PhonEngine bundled JavaScript library               | Yes; third-party library files are directly distributed                                                     |
| React                                      | PhonEngine bundled JavaScript library               | Yes; third-party library files are directly distributed                                                     |
| ReactDOM                                   | PhonEngine bundled JavaScript library               | Yes; third-party library files are directly distributed                                                     |
| Tailwind CSS                               | PhonEngine bundled JavaScript library               | Yes; third-party library files are directly distributed                                                     |
| PyCantonese                                | External software dependency                        | No                                                                                                          |
| LSHK Jyutping resources                    | CantRomZJ1 pronunciation-data source                | **Yes; the repository contains partial source content and derived content generated from it**               |
| pypinyin / related pronunciation resources | MandRomZJ1 pronunciation-data source                | **Yes; editing states / outputs contain partial source information and derived content generated from it**  |
| Multi-function Chinese Character Database  | Pronunciation-data source for several RomZJ schemes | **Yes; editing states /  outputs contain partial source information and derived content generated from it** |
| Kaom.net                                   | Supported external input source for PhonConvert     | No                                                                                                          |
| AISHELL-3                                  | Experimental speech dataset                         | No; filenames only                                                                                          |
| MDCC                                       | Experimental speech dataset                         | No; filenames only                                                                                          |
| Rime                                       | Output interoperability target                      | No                                                                                                          |
                                                                        
---

## 11. Updates and Additional Third-Party Resources

## 11. 更新及其他第三方資源

隨着 Sinitic Romanization Ecosystem 持續擴展，未來可能加入新的 third-party software dependencies、language resources、datasets 或 interoperability targets。

新增第三方內容時，contributors 應：

1. 明確記錄 upstream source；
2. 確認相應 copyright / license / terms；
3. 保留 upstream 所要求的 notices 及 attribution；
4. 說明第三方內容是否直接包含於 repository；
5. 說明哪些部分屬於本項目或 contributor 的原創 contribution；
6. 在必要時更新本文件及相關 folder-specific notices。

As the Sinitic Romanization Ecosystem continues to expand, additional third-party software dependencies, language resources, datasets, and interoperability targets may be introduced.

When adding third-party materials, contributors should:

1. clearly identify the upstream source;
2. verify the applicable copyright, license, and terms;
3. preserve required upstream notices and attribution;
4. state whether third-party content is directly distributed in the repository;
5. distinguish project-created or contributor-created components from upstream content;
6. update this document and relevant folder-specific notices where necessary.

---

如本文件與特定文件或子目錄中的 `LICENSE`、`NOTICE`、`THIRD_PARTY_NOTICES.md` 或其他更具體的授權說明存在差異，應以**最接近相關資源的具體說明及其 upstream license**為準。

If this document differs from a `LICENSE`, `NOTICE`, `THIRD_PARTY_NOTICES.md`, or other more specific licensing statement associated with a particular file or directory, the **more specific notice associated with that resource and the applicable upstream license** should govern.
