# Parallel Prediction Model Based on VMD Rolling Decomposition + Transformer-LSTM

\tPreface
As time series prediction has been widely applied in fields such as energy, finance, and meteorology, how to improve the accuracy and stability of predictions has become a research hotspot. Traditional deep learning models like LSTM are adept at capturing long-term and short-term dependencies in time series, but their performance may be limited when faced with complex nonlinear signals. On the other hand, Transformers, with their powerful self-attention mechanism, perform exceptionally well in capturing global dependencies, but lack a natural sensitivity to local temporal features. To address the limitations of single models, this issue innovatively proposes a predictive model framework based on Variational Mode Decomposition (VMD) rolling decomposition and parallel integration of Transformer-LSTM.The method uses VMD to perform multimodal decomposition on time series signals. Effectively separate multiple frequency components within the signal. Synchronize the information of different components into the multi-model architecture. Fully explore the complex dynamic characteristics of the sequence. Thus, it significantly improves the prediction performance.
\t  
● Dataset: Wind Power Power Data Set
● Environment Framework: Python 3.9, PyTorch 2.1 and above can be run.
● Usage Object: Paper requirements, graduation design requirements.
● Code Guarantee: The code comments are detailed and ready to run.
1. Model Introduction
1.1 Overall Architecture Design
Transformer-LSTM Parallel Neural Network Architecture:
The Transformer module focuses on extracting global temporal dependencies from the input, enhancing the sequence representation through multi-head self-attention and positional encoding.
The LSTM module captures the local temporal dynamics, reinforcing memory of recent information. The output feature vectors from both are combined at a fusion layer to map to the prediction target.
\t1.2 Slide window and VMD rolling decomposition
(1) Data Set Import
The wind power power dataset consists of 35,040 samples and 15 features. The target variable data is selected for visualization.
\t  
(2) VMD Rolling Decomposition
Multivariate time series data, after normalization, is divided into fixed-length sample windows using a sliding window technique to provide the foundation for VMD decomposition.
\t  
By sliding a fixed-size window over the original series, only the data within the window is decomposed. This means that the oldest data in the window is removed after each new data addition. The number of subsequences generated remains constant through this process, ensuring no data leakage. Additionally, selecting an appropriate sliding window size is crucial. A small window leads to insufficient data, resulting in lost important information and reduced prediction accuracy. Conversely, a large window increases computational complexity and running time, reduces available training data, and decreases model effectiveness.
2. Parallel Prediction Model Based on VMD+Transformer-LSTM
2.1 Set parameters and train the model
1. VMD+Transformer-LSTM prediction effect is significant, VMD rolling decomposition enhances the ability to extract multi-scale features from complex signals, combined with the parallel architecture of Transformer and LSTM, realizes the supplement of global long-short term dependencies. The experimental results fully demonstrate the effectiveness of this model in complex time series prediction such as wind power power.
2.2 Visualization of prediction results
2.3 Model evaluation
Click to download: Complete original data, Python code
Previously interesting content:
Time series prediction: Analysis and comparison of LSTM, ARIMA, Holt-Winters, SARIMA models
Wind speed prediction (I) Data introduction and preprocessing
Wind speed prediction (II) EMD-LSTM model based on Pytorch
Wind speed prediction (III) EMD-LSTM-Attention model
Wind speed prediction (IV) EMD-Transformer model based on Pytorch
Wind speed prediction (V) EMD-CNN-LSTM model based on Pytorch
Wind speed prediction (VI) EMD-CNN-GRU parallel model based on Pytorch
CEEMDAN + combination prediction model (BiLSTM-Attention + ARIMA)
CEEMDAN + combination prediction model (CNN-LSTM + ARIMA)
CEEMDAN + combination prediction model (Transformer - BiLSTM + ARIMA)
CEEMDAN + combination prediction model (CNN-Transformer + ARIMA)
Multi-feature variable sequence prediction (I) - CNN-LSTM wind speed prediction model
Multi-feature variable sequence prediction (II) - CNN-LSTM-Attention wind speed prediction model
Multi-feature variable sequence prediction (III) - CNN-Transformer wind speed prediction model
Multi-feature variable sequence prediction (IV) Transformer-BiLSTM wind speed prediction model
Multi-feature variable sequence prediction (V) CEEMDAN+CNN-LSTM wind speed prediction model
Multi-feature variable sequence prediction (VI) CEEMDAN+CNN-Transformer wind speed prediction model
Prediction model based on the SSA optimization algorithm of cuckoo: CEEMDAN-BiLSTM-Attention
Prediction model based on the SSA optimization algorithm of cuckoo: CEEMDAN-Transformer-BiGRU
Superior predictive model: Secondary decomposition-combined prediction
Multi-feature variable sequence prediction (VII) CEEMDAN+Transformer-BiLSTM prediction model
Multi-feature variable sequence prediction (VIII) Prediction model based on the SSA optimization algorithm of cuckoo: CEEMDAN-SSA-BiLSTM
Multi-feature variable sequence prediction (11) Prediction model based on Pytorch's TCN-GRU
VMD + CEEMDAN secondary decomposition, CNN-LSTM prediction model
VMD + CEEMDAN secondary decomposition, CNN-Transformer prediction model
VMD + CEEMDAN secondary decomposition, Transformer-BiGRU prediction model
Prediction model based on the SSA optimization algorithm of cuckoo: code family kit
Superior combined prediction model!
High innovation | CEEMDAN + SSA-TCN-BiLSTM-Attention prediction model
Superior combined prediction model!
Lowest price online | Family kit continuously updated!
| Based on TCN-SENet + BiGRU-GlobalAttention parallel prediction model
Secondary decomposition - innovative model prediction family kit
BiTCN-BiGRU-CrossAttention integrated spatiotemporal features high innovation prediction model
Combination Forecast Update | Superior Combination Forecast Model!
BiTCN-Transformer Parallel Forecast Model with Spatiotemporal Feature Fusion
Multi-level Attention Mechanism-Based Parallel Forecast Model
CEEMDAN-CNN-GRU-GlobalAttention + XGBoost Combination Forecast
Multi-Step Forecast Series | Collection of LSTM, CNN, Transformer, TCN, Serial, Parallel Models
End
\t2. Friends who like this can click to follow, give the article a "like", share on WeChat Moments or discuss in groups.

## Images

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
