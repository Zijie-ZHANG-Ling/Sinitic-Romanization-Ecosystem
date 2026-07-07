# Sinitic-Romanization-Ecosystem

Supplementary materials, data, and tools for an anonymized research submission on cross-lingual Sinitic romanization.

As shown by the repository timestamps and commit history, most of the code and language resources described in the paper were uploaded before the submission deadline on June 21, 2026 (AoE). Some resources and documentation were further completed and improved after the deadline, including the MandRomZJ1 homophone-character table, the corresponding PhonConvert edit-state JSON, the experimental audio-file lists, and some detailed READMEs. The repository state before the deadline can be inspected through the commit history.

For the sampled data used for the MMS fine-tuning experiment, please refer to `sampled_file_names`.

For the `PhonEngine` system with `PhonSymbol` and `PhonConvert`, please refer to the folder `PhonEngine`.

For the romanization systems of different Sinitic languages, including `PhonSymbol` scheme files and `PhonConvert` state files and homophone-character table files, please refer to the `RomZJ` naming folders. Romanization system folder names begin with the corresponding Sinitic language name. E.g., Cant for Cantonese 廣東話/穗港澳粵語, Mand for Mandarin/Modern-Standard-Chinese 國語/普通話/現代標準漢語, Nanjing for Nanjing Jianghuai Mandarin 南京江淮官話/南京話, MeixianKejia for Meixian Kejia/Hakka 梅縣客家話/梅縣話, ShanghaiWu for Shanghai Wu Chinese 上海吳語/上海話.

For the system and demo of converting `PhonConvert` homophone-character table to Rime YAML files, please refer to `convert_to_rime_yaml`.

For the open-source resources for CantRomZJ1, please refer to `cantromzj1_data` for the data part and `cantromzj1_jyutping_py` for the tool part connecting to the Jyutping ecosystem. For the PyPI release of the tools, please refer to [PySinRom](https://pypi.org/project/pysinrom/). 
