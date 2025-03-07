<style>
  h3 {
    text-align: center;
  }
</style>


# DualSpec: Text-to-spatial-audio Generation via Dual-Spectrogram Guided Diffusion Model

## Abstract
Text-to-audio (TTA), which generates audio signals from textual descriptions, has received huge attention in recent years. However, recent works focused on text to monaural audio only. As we know, spatial audio provides more immersive auditory experience than monaural audio, e.g. in virtual reality. To address this issue, we propose a text-to-spatial-audio (TTSA) generation framework named DualSpec.Specifically, it first trains variational autoencoders (VAEs) for extracting the latent acoustic representations from sound event audio. Then, given text that describes sound events and event directions, the proposed method uses the encoder of a pretrained large language model to transform the text into text features. Finally, it trains a diffusion model from the latent acoustic representations and text features for the spatial audio generation. In the inference stage, only the text description is needed to generate spatial audio. Particularly, to improve the synthesis quality and azimuth accuracy of the spatial sound events simultaneously, we propose to use two kinds of acoustic features. One is the Mel spectrograms which is good for improving the synthesis quality, and the other is the short-time Fourier transform spectrograms which is good at improving the azimuth accuracy. We provide a pipeline of constructing spatial audio dataset with text prompts, for the training of the VAEs and diffusion model. We also introduce new spatial-aware evaluation metrics to quantify the azimuth errors of the generated spatial audio recordings. Experimental results demonstrate that the proposed method can generate spatial audio with high directional and event consistency.

## Demos
We showcase ​DualSpec's spatial audio generation capabilities through three direction descriptors.: 1) ​Direction-of-Arrival (DOA)​, 2) ​Clock Position​, and 3) ​General Description.

## Direction-of-Arrival (DOA)

<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/doa/248790^0_true0_pred0.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">woodwind & DOA 60°</p>
  </div>
  
  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/doa/94370^270_true270_pred270.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">walk and footsteps & DOA 270°</p>
  </div>

  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/doa/18581-3-0-5^180_true180_pred180.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">dog bark & DOA 180°</p>
  </div>
</div>

<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/doa/1-30214-A-18^300_true300_pred300.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">toilet flush & DOA 300°</p>
  </div>
  
  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/doa/12775^0_true0_pred0.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">pinao & DOA 0°</p>
  </div>

  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/doa/2-95258-A-1^210_true210_pred210.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">rooster & DOA 210°</p>
  </div>
</div>

<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/doa/3-144253-A-29^60_true60_pred60.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">drinking & DOA 60°</p>
  </div>
  
  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/doa/3471^150_true150_pred150.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">acoustic guitar & DOA 150°</p>
  </div>

  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/doa/4-204777-B-39^180_true180_pred180.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">glass breaking & DOA 180°</p>
  </div>
</div>

## Clock Position

<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/time/4-187769-B-14^0_true0_pred0.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">chirping birds & 12 o'clock direction</p> 
  </div>
  
  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/time/130586^270_true270_pred270.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">wind chime & 3 o'clock direction</p>
  </div>

  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/time/18772^150_true150_pred150.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">accelerating and revving & 7 o'clock direction</p>
  </div>
</div>

<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/time/1-104089-A-22^300_true300_pred300.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">clapping & 2 o'clock direction</p>
  </div>
  
  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/time/1-79113-A-5^60_true60_pred60.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">baby crying & 10 o'clock direction</p>
  </div>

  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/time/114587-3-0-7^120_true120_pred120.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">dog bark & 8 o'clock direction</p>
  </div>
</div>

<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/time/11970^180_true180_pred180.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">guitar & 6 o'clock direction</p>
  </div>
  
  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/time/135703^0_true0_pred0.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">electric guitar & 12 o'clock direction</p>
  </div>

  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/time/2-135649-B-45^210_true210_pred210.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">train & 5 o'clock direction</p>
  </div>
</div>

## General Description

<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/rough/371813^30_true30_pred30.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">bathhub washing & forward left, slight angle</p>
  </div>
  
  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/rough/248434^150_true150_pred150.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">woodwind & positioned to the rear on the left side</p>
  </div>

  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/rough/377021^210_true210_pred210.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">applause & rear, slightly to the right</p>
  </div>
</div>

<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/rough/115242-9-0-68^240_true240_pred240.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">street music & rear right</p>
  </div>
  
  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/rough/3-134049-A-1^180_true180_pred180.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">rooster & directly behind</p>
  </div>

  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/rough/35286^60_true60_pred60.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">cowbell & toward the front left</p>
  </div>
</div>

<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/rough/4-187769-B-14^0_true0_pred0.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">chirping birds & straight head</p>
  </div>
  
  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/rough/4-250869-C-2^210_true210_pred210.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">pig & right rear</p>
  </div>

  <div style="margin: 10px;">
    <audio controls>
      <source src="audio/rough/5-250026-A-30^300_true300_pred300.wav" type="audio/wav">
      Your browser does not support the audio element.
    </audio>
    <p style="text-align: center;">knock & to the right front, slightly moving back</p>
  </div>
</div>
