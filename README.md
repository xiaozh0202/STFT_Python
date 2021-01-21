# STFT_Python
Short-time Fourier transform (STFT) effect in MATLAB is realized by Python code（利用Python代码实现matlab中的短时傅里叶变换效果）


Use"pip install -r requirements.txt" to install the dependent libraries.


Use such a command:
"python pystft.py -wp test.wav -sp test.png -l 8192 -o 7168"

Parameter description:  


English：  
"-wp", "--wavepath", "The path to the audio file"，Required parameters；  
"-sp", "--savepath", "The path the image needs to be saved"，Required parameters；  
"-s", "--size", "Size of picture",Optional parameters，default=224,The length is the same as the width；  
"-sr", "--samplerate", "The sampling rate of audio", Optional parameters，default=44100,**PCM file needs to fill in the sampling rate**, WAV can not fill；  
"-l", "--length", "The window length of STFT"，Required parameters；  
"-o", "--overlap", "The overlap length of STFT"，Required parameters,length-overlap=step；  
"-w", "--window", "The window function of STFT",Optional parameters，default="hamm"；  
"-n", "--normali", "Data normalization", Optional parameters，default=True.  


中文版：  
"-wp", "--wavepath", "音频文件路径"，必填参数；  
"-sp", "--savepath", "图片保存的路径"，必填参数；  
"-s", "--size", "图片的大小",可选参数，默认=224，长和宽一样；  
"-sr", "--samplerate", "音频文件采用频率", 可选参数，默认=44100,pcm文件需要填写采样率，wav可以不填；  
"-l", "--length", "STFT窗口大小"，必填参数；  
"-o", "--overlap", "STFT的overlap大小"，必填参数，length-overlap=step；  
"-w", "--window", "STFT使用的窗函数",可选参数，默认="hamm"；  
"-n", "--normali", "数据归一化", 可选参数，默认=True。
