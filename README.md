# Transparent pronunciation scoring using articulatorily weighted phoneme edit distance

Compendium for the paper by Karhila, Smolander, Ylinen &amp; Kurimo submitted to Interspeech 2019

Contents:
- [Long list of audio files](corpus_dataset_filename.txt) used to train the recogniser
- [Python pickle of N-best hypotheses of recognition results and assorted metadata](phone_recognition_results_v0.22.pickle)
- [phoneset.html](phoneset.html) Description of the used phoneme set ( [html preview](https://htmlpreview.github.io/?https://github.com/aalto-speech/interspeech2019_karhila_et_al/blob/master/phoneset.html) )
- [scoring_experiment.ipynb](scoring_experiment.ipynb) Jupyter notebook for running the scoring experiment

After running the experiments several times, the results for correlations of predicted scores to human annotations are:


| Method                  | Correlation (all) | Correlation (outliers removed)  |
| ----------------- | --------------- | ---------------------- |
| Baseline PWLD     |  0.43 ± 0.00    |  0.47 ± 0.00           |
| Data-driven PWLD  |  0.47 ± 0.00    |  0.53 ± 0.01           |
| Random Forest     |  0.50 ± 0.00    |  0.54 ± 0.01           |
| Support Vector    |  0.51 ± 0.02    |  0.55 ± 0.04           |
