### Download Turkish female and male speech datasets from Mozilla Common Voice for speech synthesis (TTS) systems

This repository provides Turkish voice datasets of male and female speakers from Mozilla Common Voice, public audio data that you can download for speech synthesis systems.

Source Dataset | Language | Gender | # of Sentences | Size (Hours) |
 ------- | ------- | ------- | ------- | ------- |  
[Common Voice Corpus 11.0](https://commonvoice.mozilla.org/tr/datasets)| Turkish | Female (1 speaker)| 9960 | 9.35 |
[Common Voice Corpus 11.0](https://commonvoice.mozilla.org/tr/datasets) | Turkish | Male (1 speaker)| 4999 | 3.09 |

### Download Speech Data for Any Languages for Specific Speaker

- In the following script `download_tr_female_and_male_speaker_audios.ipynb` change the version and language to you wish to download from 
[Mozilla](https://commonvoice.mozilla.org/en/datasets).
```python
version = 'cv-corpus-11.0-2022-09-21'
language = 'cv-corpus-11.0-2022-09-21-tr'
```

You can list speakers who have the most recorded audios.
```
Client ID: ba25f19f22267b1f863cef586f17252a9067bc0ecb3d63dd7626fbce7014a16412dd64d5404d34505c0c90635adbc3cb2d830d77291a4db194e5abad91160957 | Gender: female | Count: 17252
Client ID: 6cf4dea5df1dfe5dc5d7bacdb6da105b9e48e01fd0f069dbaf0ad906a7c5d78032194a3a9384e8589b93c58a04a12f676669f4c4501e52cee652f331b72b9205 | Gender: female | Count: 17194
Client ID: c3c204ffaebfc46c0265773376f9288a372694aa79f97afe224828033c28d6d2a90919aaf769bf14105cb4033650e10275760afe250490782eae15c1d1518799 | Gender: male | Count: 6349
Client ID: 60cee2235d7ec4cdeb89d601b8c373955b303c712ec729ed0affdabda8819908f51cefa990163d2bc4ac04c93e6dac2909cca67829211df4a2a17af2507dd50a | Gender: male | Count: 6291
Client ID: ca179eb54e4e584d30587ba3c6c1d4de7d9082d649113d481d308f3e7d858e0a1df21d9591f9c613928b1e122aa7f54535d0f0e0c1380d87d8017844e6e73ea2 | Gender: male | Count: 4837
```

- Choose the speaker ID that you want to download the dataset.
```python
female_rank = input("Choose the ID number rank for the female voice dataset:")
male_rank = input("Choose the ID number rank for the male voice dataset:")
```

- Finally you can download `./CommonVoice_dataset/female_data/wav/` and `./CommonVoice_dataset/male_data/wav/` datasets;
create `./commonvoice_female_data_manifest.jsonl` and `./commonvoice_female_data_manifest.jsonl/` manifest files.

```python
Female voice dataset total duration:9.35 hours
Male voice  dataset total duration:3.09 hours
```
