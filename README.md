Isolated Word Speech Recognition Based on STM32

This design studies the isolated word speech recognition system and its implementation on the STM32 embedded platform. 
The identification process is: pre-filtering, ADC, framing, endpoint detection, pre-emphasis, windowing, feature extraction, feature matching. Endpoint Detection (VAD) combines a short-term amplitude with a short-term zero-crossing rate. 
After the effective speech is detected, the Mel frequency cepstral coefficient (MFCC) of each frame of speech is calculated according to the auditory perception characteristics of the human ear. 
Then use the dynamic time warping (DTW) algorithm to match the feature template, and finally output the recognition result. Firstly, the above algorithm is simulated by Matlab. 
After many experiments, the optimal values of the coefficients required in the algorithm are obtained. 
Then the algorithm is transplanted to the STM32 embedded platform. 
During the migration process, the algorithm is optimized according to the actual situation that the embedded platform has relatively small storage space and relatively weak computing power. 
Finally, an STM32-based isolated speech recognition system was designed and produced.

####Details:
Http://gk969.com/stm32-speech-recognition/
