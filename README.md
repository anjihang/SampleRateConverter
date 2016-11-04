# SampleRateConverter
A simple audio sample rate converter

# 说明
- 这是一个基于相似三角形性质的近似采样率转换算法，可以将任意采样率的音频转换成其他任意的采样率，能用在精度不高，但需要处理速度快的场合。
- 此算法处理的结果在低频范围内的频率分布基本和Cool Edit软件处理的效果一致，但高频部分可能有损失。
- 由于只用直线估计实际采样点之间的采样值，没有滤波过程，此算法的时间复杂度只有O(n)。
- 在我的PC上运用此算法，3分钟的音频文件从44.1K转到48K只需处理1秒左右；而同一环境下，Cool Edit需要处理近半分钟。
- wav文件读写的类来源于https://github.com/sintrb/WaveAccess/tree/master/src/com/sin/java/waveaccess

#Description
- This is an approximate sample rate conversion algorithm based on similar triangular properties that can convert arbitrary sample rate audio to other arbitrary sample rates and can be used in situations where accuracy is not high but processing speed is high.
- The results of this algorithm in the low frequency range of the frequency distribution, basically the same effect with the Cool Edit software processing, but there may be loss of high-frequency part.
- Since only straight lines are used to estimate the sampled values between the actual sampling points and there is no filtering process, the time complexity of this algorithm is only O (n).
- In my PC on the use of this algorithm, 3 minutes of audio files from 44.1K to 48K  only need to deal with about 1 second. The same environment, Cool Edit need to deal with nearly half a minute.
- Wav file read and write classes are from https://github.com/sintrb/WaveAccess/tree/master/src/com/sin/java/waveaccess
