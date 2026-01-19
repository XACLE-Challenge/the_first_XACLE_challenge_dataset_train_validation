# XACLE Challenge 2026 dataset training and validation set

## Contents

This dataset consists of the following componets:

- Audio–text pairs

	This dataset includes 7,500 audio–text pairs for training and 3,000 audio–text pairs for validation.
	Each text is written in English.
	All audio samples was converted to mono 16-bit 16 kHz format.

- 11-point semantic-alignment scores between audio and text (per listener)

	This dataset includes subjective evaluation scores for semantic alignment between audio and text.
	The semantic-alignment score is on a an 11-point scale from 0 ("does not match at all") to 10 ("matched exactly").
	Each audio–text pair is evaluated by four native English-speaking .

- Average semantic-alignment scores
	
	This dataset includes average semantic-alignment scores for each audio–text pair.

- Listener IDs

	This dataset includes listener IDs of those who scored the semantic alignment between audio and text.

## Download

To download the dataset, please send an email to dataset@xacle.org with “Download dataset” in the subject line. 
You will receive an automated reply with the download link.
<b>If you don't receive a reply after a while, please check your spam folder. If the email fails to send or you still don't receive a reply, please contact the organizer at y-oka@g.ecc.u-tokyo.ac.jp.<b>


## Statistics

|  | Train | Validation |
| :--- | ---: | ---: |
| Evaluations | 30,000 |  12,000 |
| Audio–text pairs | 7,500 |  3,000 |
| Audio duration [s] | 75,000 | 30,000 |
| Listeners | 2,323 | 668 |

## File format

- [train,validation].csv: There are 4 columns in the each csv file.
	- wave_file_name: The file name of audio.
	- text: The text's corresponding audio.
	- 11-point semantic-alignment score: The evaluation scores for semantic alignment between audio and text by each listener.
	- listener_id: The listener ID who scored the sematic-alignment scores.

- [train_average,validation_average].csv: There are 3 columns in the each csv file.
	- wave_file_name: The file name of audio.
	- text: The text's corresponding audio.
	- average_semantic_alignement_score: The average semantic-alignment scores of each audio-text pair.

## Directory structure

The directory structure of this dataset is as follows:

```
XACLE_dataset
├── meta_data
│   ├── train_average.csv
│   ├── train.csv
│   ├── validation_average.csv
│   └── validation.csv
└── wav
    ├── train
    │   ├── 00000.wav
    │   ├── 00001.wav
    │   ├── 00002.wav
    │   ├──   .
    │   ├──   .
    │   └──   .
    └── validation
        ├── 07500.wav
        ├── 07501.wav
        ├── 07502.wav
        ├──   .
        ├──   .
        └──   .
```

## Citation

Please cite the paper that will be uploaded to arXiv in early November, 2025.

## Acknowledgment

The work was supported by JSPS KAKENHI Grant Number 24K23880, 25K21221, JST Moonshot Grant Number JPMJMS2237.

