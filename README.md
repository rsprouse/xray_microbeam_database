# xray_microbeam_database
Annotations and scripts for use with the [University of Wisconsin X-Ray Microbeam Speech Production Database (1994) dataset](https://berkeley.box.com/v/xray-microbeam-database-data). 

## Citation for the Wisconsin X-Ray Microbeam Speech Production Database

Westbury, John with Greg Turner and Jim Dembowski (1994) X-Ray Microbeam Speech Production Database User’s Handbook, v. 1.0, Waisman Center on Mental Retardation & Human Development, Univ. of Wisconsin, Madison, WI.

## `.csv` files

Four `.csv` files in the `annotation` folder are compiled from tables in the 'X-Ray Microbeam Speech Production Database User's Handbook` (ubdbman.pdf) distributed with the data files (not in this repository; see dataset link above):

- `speaker_demographics1.csv`: Table 4.1: Demographics (p. 21)
- `speaker_demographics2.csv`: Table 4.2: Place of Birth (POB), Dialect Base (DB), and Residence (Res) (p. 22)
- `speaker_dental_info1.csv`: Table 4.3: Dental information I (p. 25)
- `speaker_dental_info2.csv`: Table 4.4: Dental information II (p. 26)

An additional two `.csv` files contain all of the labels in all of the textgrids in precompiled form. The `all_phones.csv` file contains all labels from the textgrid `phone` tiers, and `all_words.csv` all labels from the textgrid `word` tiers. The fields in these `.csv` files are:

- `t1`: start time of label
- `t2`: end time of label
- `phone` (`all_phones.csv`) / `word` (`all_words.csv`): label text
- `speaker`: the speaker of the utterance
- `uttid`: the utterance identifier portion of the audio filename, e.g. 'tp001'
- `rep`: the repetition number for the utterance (found after underscore ('_') in the audio filname for values greater than 1), e.g. 'tp015_2'
- `wavpath`: the path to the `.wav` file where the audio corresponding to the phone/word label can be found

