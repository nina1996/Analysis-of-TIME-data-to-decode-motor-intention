# Analysis-of-TIME-data-to-decode-motor-intention
Created by Nikolina Tomic, Feb-July 2020

The purpose of this project was to explore the potential of electroneurography (ENG) signals recorded from inside of nerve fibers by using deep learning.

Few different perspectives are combined in this project, as aim was to get insight in qualitative properties of TIMEs signals. 4 movements, followed by rest phase were defined and corresponding ENG signals provided. Signals are first cleaned from artifacts and downsampled. Classification and regression targets are created and this project is then driven by two main ideas: 1. preprocess the signals and decode features representation; 2. decode the original, raw signals. In the former case, decode stands for classification, while in the latter for regression.
Preprocessing is done by calculating Root Mean Square (RMS) of the signals. The NN classification approach is then performed for intra-session and inter-session data split.

Besides NN, CNN on preprocessed-data is also tested, again in both intra-session and inter-session fashion. Kolomgorov-Smirnov test is applied in order to analyse features properties, and to compare intra-session and inter-session capabilities. Last step was to test performance of CNN-regression approach on raw signals as the idea was to test the same pipeline widely used in EMG signal processing, i.e. creating images from RAW data and performing CNN, while doing regression rather than classification. This is, again done in intra-session and inter-session fashion.

  Please refer to Report.pdf for more details.
