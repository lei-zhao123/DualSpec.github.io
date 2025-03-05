
<style>
  h3 {
    text-align: center;
  }
</style>


# DualSpec: Text-to-spatial-audio Generation via Dual-Spectrogram Guided Diffusion Model

## Abstract
Text-to-audio (TTA), which generates audio signals from textual descriptions, has received huge attention in recent years. However, recent works focused on text to monaural audio only. As we know, spatial audio provides more immersive auditory experience than monaural audio, e.g. in virtual reality. To address this issue, we propose a text-to-spatial-audio (TTSA) generation framework named DualSpec.Specifically, it first trains variational autoencoders (VAEs) for extracting the latent acoustic representations from sound event audio. Then, given text that describes sound events and event directions, the proposed method uses the encoder of a pretrained large language model to transform the text into text features. Finally, it trains a diffusion model from the latent acoustic representations and text features for the spatial audio generation. In the inference stage, only the text description is needed to generate spatial audio. Particularly, to improve the synthesis quality and azimuth accuracy of the spatial sound events simultaneously, we propose to use two kinds of acoustic features. One is the Mel spectrograms which is good for improving the synthesis quality, and the other is the short-time Fourier transform spectrograms which is good at improving the azimuth accuracy. We provide a pipeline of constructing spatial audio dataset with text prompts, for the training of the VAEs and diffusion model. We also introduce new spatial-aware evaluation metrics to quantify the azimuth errors of the generated spatial audio recordings. Experimental results demonstrate that the proposed method can generate spatial audio with high directional and event consistency.

## Demos
We showcase ​DualSpec's spatial audio generation capabilities across three descriptive paradigms: 1) ​Direction-of-Arrival (DOA)​ with angular precision (e.g., "Helicopter traversing 120°→240°"), 2) ​Clock Position​ for intuitive localization (e.g., "at 3 o'clock"), and 3) ​Rough Directional​ scenarios with environmental immersion (e.g., "Car passing behind listener").

## Direction-of-Arrival (DOA)

### mel
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <audio controls>
      <source src="mel/doa/248790^0_true0_pred0.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>
  
  <div style="margin: 10px;">
    <audio controls>
      <source src="mel/doa/94370^270_true270_pred270.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>

  <div style="margin: 10px;">
    <audio controls>
      <source src="mel/doa/18581-3-0-5^180_true180_pred180.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>
</div>

### twoconcat
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <audio controls>
      <source src="twoconcat/doa/audio1.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>
  
  <div style="margin: 10px;">
    <audio controls>
      <source src="twoconcat/doa/audio2.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>

  <div style="margin: 10px;">
    <audio controls>
      <source src="twoconcat/doa/audio3.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>
</div>

### twoconcat2
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <audio controls>
      <source src="twoconcat2/doa/audio1.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>
  
  <div style="margin: 10px;">
    <audio controls>
      <source src="twoconcat2/doa/audio2.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>

  <div style="margin: 10px;">
    <audio controls>
      <source src="twoconcat2/doa/audio3.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>
</div>

## Clock Position

### mel
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <audio controls>
      <source src="mel/time/4-187769-B-14^0_true0_pred0.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>
  
  <div style="margin: 10px;">
    <audio controls>
      <source src="mel/time/130586^270_true270_pred270.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>

  <div style="margin: 10px;">
    <audio controls>
      <source src="mel/time/18772^150_true150_pred150.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>
</div>

### twoconcat
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <audio controls>
      <source src="twoconcat/clock/audio1.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>
  
  <div style="margin: 10px;">
    <audio controls>
      <source src="twoconcat/clock/audio2.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>

  <div style="margin: 10px;">
    <audio controls>
      <source src="twoconcat/clock/audio3.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>
</div>

### twoconcat2
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <audio controls>
      <source src="twoconcat2/clock/audio1.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>
  
  <div style="margin: 10px;">
    <audio controls>
      <source src="twoconcat2/clock/audio2.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>

  <div style="margin: 10px;">
    <audio controls>
      <source src="twoconcat2/clock/audio3.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>
</div>

## Rough Directional

### mel
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <audio controls>
      <source src="mel/rough/371813^30_true30_pred30.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>
  
  <div style="margin: 10px;">
    <audio controls>
      <source src="mel/rough/248434^150_true150_pred150.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>

  <div style="margin: 10px;">
    <audio controls>
      <source src="mel/rough/377021^210_true210_pred210.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>
</div>

### twoconcat
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <audio controls>
      <source src="twoconcat/rough/audio1.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>
  
  <div style="margin: 10px;">
    <audio controls>
      <source src="twoconcat/rough/audio2.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>

  <div style="margin: 10px;">
    <audio controls>
      <source src="twoconcat/rough/audio3.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>
</div>

### twoconcat2
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <audio controls>
      <source src="twoconcat2/rough/audio1.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>
  
  <div style="margin: 10px;">
    <audio controls>
      <source src="twoconcat2/rough/audio2.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>

  <div style="margin: 10px;">
    <audio controls>
      <source src="twoconcat2/rough/audio3.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">[Caption placeholder]</p>
  </div>
</div>
