# Sequential Modeling of Classical Music Generation

## Abstract
In this project, we want to investigate whether sequential models (previously implemented in Kalman Filter or RNN, LSTM) could serve as good modules for existing music generation tasks. In other words, we want to know if the generation results from these models trained causally on the former notes are close to the ground truth notes in the future. Also, we are interested in comparing the generation performance between Kalman Filtering as an unsupervised algorithm with LSTM as a supervised one. 

This study explores Kalman Filtering and LSTM models for music generation, highlighting their strengths and limitations. Kalman Filtering proves to be a strong candidate, delivering competitive acoustic results similar to LSTM models. While its initial guess influences early note generation and requires more time to converge with random initialization, it excels in adaptability, aligning with music patterns even from poor estimates. Its lightweight design, real-time prediction, and ability to handle tempo changes make it ideal for dynamic settings, though it faces challenges with parameter sensitivity, weaker long-term predictions, and linear assumptions.

LSTM models, on the other hand, excel at capturing long-term dependencies and generating complex harmonies but come with high computational costs and training complexity. Additionally, we observe that standard metrics often fail to align with human perceptions of musical quality, underscoring the need for subjective evaluations or improved metrics. This study highlights the trade-offs between Kalman Filtering’s real-time adaptability and LSTM’s complexity, providing insights into their application in sequential music generation.

## Dataset
This dataset comprises MIDI files of classical piano compositions by 19 renowned composers, originally curated from the website \url{http://www.piano-midi.de}. The dataset features a selection of 295 MIDI files, encompassing a variety of pieces and movements from composers such as Bach, Chopin, Mozart, and Schubert among others.

The MIDI files in this dataset represent a wide range of classical music styles and periods, providing a rich source of data for analyzing musical patterns, styles, and structures across different composers and historical contexts. Each file corresponds to a specific musical composition, with some files containing individual movements or sections of larger works. This diversity allows for a comprehensive study of the elements that define classical piano music.

The use of MIDI files is particularly advantageous for musical analysis as they contain precise information about the notes, timings, and dynamics of the performance, making them ideal for detailed computational analysis aimed at understanding and modeling classical music composition and performance practices.

## For Data Preprocessing, Pipeline, Modelngs, and Results
Check Report.pdf
