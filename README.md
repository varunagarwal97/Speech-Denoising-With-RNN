# Speech-Denoising-With-RNN
Speech Denoising using RNNs in Tensorflow

Through this project, you can get an idea about denoising speech signals using RNNs in Tensorflow. You should have a basic idea as to what an STFT does and what Ideal binary masks are, in order to understand the why of what I am doing here (will post a brief introduction soon). 

This project constructs a Recurrent neural network to denoise speech signals with varying kinds of noises in each of the training signals. The architecture of the network uses LSTM cells to learn to denoise the signals. 

For training, we started with the noisy speech signal (X), the corresponding noise signal (N), and the clean speech signal (S). We then compute the Ideal Binary Masks (IBM) from the clean speech signal and the noise signal. The IBMs are what the RNN learns to predict which are then converted back into speech signals. 

On the validation set I managed an average SNR of 10 dB, which is decent for a fairly simpler model. 

Will be uploading the dataset soon, so that you can listen and enjoy the recovered signals. Till then try to play around with the code.
