We take the `MeixianKejiaRomZ2` as an example here.

Using `MeixianKejiaRomZJ2_同音字表_20260506_134059.csv` as the input file for the `HTML` converting frontend, you can get `MeixianKejiaRomZJ2_rime_files.zip` (or `.zip` file with other name defined by you, the `.zip` file naming convension is {your entered `SCHEMA ID`}+'_rime_files') as the output file generated.

You can also use the `Python` script to implement the conversion. Arguments are needed to run the script in cmd/Terminal. The arguments are:

```
    parser.add_argument("csv_path", type=Path, help="Input homophone-character CSV file.")
    parser.add_argument("-o", "--output-dir", type=Path, default=Path("rime_output"), help="Output directory.")
    parser.add_argument("--schema-id", default="romzj_input", help="Rime schema id. Use ASCII lowercase/underscore.")
    parser.add_argument("--schema-name", default="RomZJ Input", help="Display name of the Rime schema.")
    parser.add_argument("--version", default="0.1.0", help="Version string for generated YAML files.")
```
