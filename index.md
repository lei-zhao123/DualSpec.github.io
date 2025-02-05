<style>
  h3 {
    text-align: center;
  }
</style>


# UniForm: A Unified Diffusion Transformer for Audio-Video Generation

## Abstract
As a natural multimodal content, audible video delivers an immersive sensory experience. Consequently, audio-video generation systems have substantial potential. However, existing diffusion-based studies mainly employ relatively independent modules for generating each modality, which lack exploration of shared-weight generative modules. This approach may under-use the intrinsic correlations between audio and visual modalities, potentially resulting in sub-optimal generation quality. To address this, we propose UniForm, a unified diffusion transformer designed to enhance cross-modal consistency. By concatenating auditory and visual information, UniForm learns to generate audio and video simultaneously within a unified latent space, facilitating the creation of high-quality and well-aligned audio-visual pairs. Extensive experiments demonstrate the superior performance of our method in joint audio-video generation, audio-guided video generation, and video-guided audio generation tasks.

## Demos
We present generation results from our proposed **UniForm** across multiple audio-video synthesis conditions. Each set demonstrates three key capabilities under identical labels or captions: text-to-audible video (T2AV), audio-to-video (A2V), and video-to-audio (V2A).

## Landscape

### fire crackling
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="audioset\ajMa6azANNw_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="audioset\ajMa6azANNw_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="audioset\ajMa6azANNw_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>
