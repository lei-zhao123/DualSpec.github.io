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

### splashing water
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="landscape\bUntI90An-U_clip_1_17fps_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="landscape\bUntI90An-U_clip_1_17fps_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="landscape\bUntI90An-U_clip_1_17fps_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

### squishing water
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="landscape\KljCauisAFc_clip_1_17fps_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="landscape\KljCauisAFc_clip_1_17fps_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="landscape\KljCauisAFc_clip_1_17fps_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

### fire crackling
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="landscape\O5zASuld4k_clip_1_17fps_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="landscape\O5zASuld4k_clip_1_17fps_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="landscape\O5zASuld4k_clip_1_17fps_v2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

### underwater bubbling
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="landscape\pNC1gD5jKIM_clip_2_17fps_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="landscape\pNC1gD5jKIM_clip_2_17fps_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="landscape\pNC1gD5jKIM_clip_2_17fps_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

### raining
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="landscape\ZxGqX1cJdSQ_clip_1_17fps_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="landscape\ZxGqX1cJdSQ_clip_1_17fps_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="landscape\ZxGqX1cJdSQ_clip_1_17fps_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>



## AudioSet

### audioset1
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

### audioset2
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="audioset\ChFCmNGP9XM_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="audioset\ChFCmNGP9XM_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="audioset\ChFCmNGP9XM_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

### audioset3
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="audioset\oRcqtJt0_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="audioset\oRcqtJt0_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="audioset\oRcqtJt0_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

### audioset4
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="audioset\xEtchO2CQBA_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="audioset\xEtchO2CQBA_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="audioset\xEtchO2CQBA_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

### audioset5
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="audioset\ZBaYrfz5afo_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="audioset\ZBaYrfz5afo_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="audioset\ZBaYrfz5afo_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>



## VGGSound

### vggsound1
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="vgg\3Kv4fdm7Uk_000030_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="vgg\3Kv4fdm7Uk_000030_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="vgg\3Kv4fdm7Uk_000030_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

### vggsound2
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="vgg\79qo5MUYBk_000207_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="vgg\79qo5MUYBk_000207_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="vgg\79qo5MUYBk_000207_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

### vggsound3
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="vgg\86gl1hp1Aw_000105_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="vgg\86gl1hp1Aw_000105_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="vgg\86gl1hp1Aw_000105_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

### vggsound4
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="vgg\615mGonUqU_000232_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="vgg\615mGonUqU_000232_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="vgg\615mGonUqU_000232_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

### vggsound5
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="vgg\AMsYmKRnWE_000008_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="vgg\AMsYmKRnWE_000008_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="vgg\AMsYmKRnWE_000008_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

### vggsound6
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="vgg\fAVezaAX18_000126_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="vgg\fAVezaAX18_000126_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="vgg\fAVezaAX18_000126_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

### vggsound7
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="vgg\GW1J75oAKU_000304_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="vgg\GW1J75oAKU_000304_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="vgg\GW1J75oAKU_000304_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

### vggsound8
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="vgg\JGpAlLrSD0_000458_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="vgg\JGpAlLrSD0_000458_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="vgg\JGpAlLrSD0_000458_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

### vggsound9
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="vgg\lPXTBXa0tE_000030_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="vgg\lPXTBXa0tE_000030_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="vgg\lPXTBXa0tE_000030_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

### vggsound10
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="vgg\YfaQljuwwA_000030_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="vgg\YfaQljuwwA_000030_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="vgg\YfaQljuwwA_000030_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

### vggsound11
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="vgg\yicwYUKKuo_000304_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="vgg\yicwYUKKuo_000304_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="vgg\yicwYUKKuo_000304_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

### vggsound12
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="vgg\Z1ZSWDouUU_000030_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="vgg\Z1ZSWDouUU_000030_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="vgg\Z1ZSWDouUU_000030_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

### vggsound13
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="vgg\zQm4CQVWqzw_000174_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="vgg\zQm4CQVWqzw_000174_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="vgg\zQm4CQVWqzw_000174_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

### vggsound14
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="vgg\zra3SOgAsyg_000031_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="vgg\zra3SOgAsyg_000031_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="vgg\zra3SOgAsyg_000031_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

### vggsound15
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="vgg\ZRVktsXO9FI_000066_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="vgg\ZRVktsXO9FI_000066_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="vgg\ZRVktsXO9FI_000066_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

### vggsound16
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="vgg\ZuBxMCk0cco_000140_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="vgg\ZuBxMCk0cco_000140_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="vgg\ZuBxMCk0cco_000140_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>

### vggsound17
<div style="display: flex; flex-wrap: wrap; justify-content: space-around; margin-bottom: 30px;">
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">T2AV</h3>
    <video width="256" height="256" controls>
      <source src="vgg\zw4X8p5zVZE_000023_t2av.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
  
  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">A2V</h3>
    <video width="256" height="256" controls>
      <source src="vgg\zw4X8p5zVZE_000023_ta2v.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>

  <div style="margin: 10px;">
    <h3 style="font-size: 18px;">V2A</h3>
    <video width="256" height="256" controls>
      <source src="vgg\zw4X8p5zVZE_000023_tv2a.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
  </div>
</div>