# Fine Tune Transcription Whisper Notebook

Notes on usage:

- Make sure to [change runtime to GPU](https://www.tutorialspoint.com/google_colab/google_colab_using_free_gpu.htm). 
- The transcript will be saved in Files, which you can find in the menu on the left.
- Change the number of speakers below if different from two.
- Pick a bigger model if you want more accuracy and a smaller model if you want the program to run faster ([more info](https://github.com/openai/whisper#available-models-and-languages)).
- If you know the language being spoken is English, then change language to 'English' as this improves performance.


High level overview of what's happening here:


1.   I'm using Open AI's Whisper model to seperate audio into segments and generate transcripts.
2.   I'm then generating speaker embeddings for each segments.
3.   Then I'm using agglomerative clustering on the embeddings to identify the speaker for each segment.   

Let me know if I can make it better!
