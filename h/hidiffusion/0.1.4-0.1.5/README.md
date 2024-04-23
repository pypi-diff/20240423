# Comparing `tmp/hidiffusion-0.1.4.tar.gz` & `tmp/hidiffusion-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hidiffusion-0.1.4.tar", last modified: Tue Apr 16 08:23:53 2024, max compression
+gzip compressed data, was "hidiffusion-0.1.5.tar", last modified: Tue Apr 23 14:21:35 2024, max compression
```

## Comparing `hidiffusion-0.1.4.tar` & `hidiffusion-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-16 08:23:53.608580 hidiffusion-0.1.4/
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)       35 2024-04-16 08:22:52.000000 hidiffusion-0.1.4/MANIFEST.in
--rw-r--r--   0 zhangshen (10250) zhangshen (10250)    14898 2024-04-16 08:23:53.608580 hidiffusion-0.1.4/PKG-INFO
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)    14605 2024-04-16 08:21:34.000000 hidiffusion-0.1.4/README.md
-drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-16 08:23:53.608580 hidiffusion-0.1.4/hidiffusion/
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      118 2024-04-16 08:21:34.000000 hidiffusion-0.1.4/hidiffusion/__init__.py
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)   103957 2024-04-16 08:21:34.000000 hidiffusion-0.1.4/hidiffusion/hidiffusion.py
-drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-16 08:23:53.608580 hidiffusion-0.1.4/hidiffusion/sd_module_key/
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)    30444 2024-04-16 08:21:34.000000 hidiffusion-0.1.4/hidiffusion/sd_module_key/sd15_module_key.txt
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)   100878 2024-04-16 08:21:34.000000 hidiffusion-0.1.4/hidiffusion/sd_module_key/sdxl_module_key.txt
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      872 2024-04-16 08:21:34.000000 hidiffusion-0.1.4/hidiffusion/utils.py
-drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-16 08:23:53.608580 hidiffusion-0.1.4/hidiffusion.egg-info/
--rw-r--r--   0 zhangshen (10250) zhangshen (10250)    14898 2024-04-16 08:23:53.000000 hidiffusion-0.1.4/hidiffusion.egg-info/PKG-INFO
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      334 2024-04-16 08:23:53.000000 hidiffusion-0.1.4/hidiffusion.egg-info/SOURCES.txt
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)        1 2024-04-16 08:23:53.000000 hidiffusion-0.1.4/hidiffusion.egg-info/dependency_links.txt
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)       12 2024-04-16 08:23:53.000000 hidiffusion-0.1.4/hidiffusion.egg-info/top_level.txt
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)       38 2024-04-16 08:23:53.608580 hidiffusion-0.1.4/setup.cfg
--rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      493 2024-04-16 08:22:44.000000 hidiffusion-0.1.4/setup.py
+drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-23 14:21:35.217582 hidiffusion-0.1.5/
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)       35 2024-04-23 14:20:01.000000 hidiffusion-0.1.5/MANIFEST.in
+-rw-r--r--   0 zhangshen (10250) zhangshen (10250)    15069 2024-04-23 14:21:35.217582 hidiffusion-0.1.5/PKG-INFO
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)    14776 2024-04-23 14:19:45.000000 hidiffusion-0.1.5/README.md
+drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-23 14:21:35.213582 hidiffusion-0.1.5/hidiffusion/
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      118 2024-04-23 14:19:45.000000 hidiffusion-0.1.5/hidiffusion/__init__.py
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)   105456 2024-04-23 14:19:45.000000 hidiffusion-0.1.5/hidiffusion/hidiffusion.py
+drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-23 14:21:35.217582 hidiffusion-0.1.5/hidiffusion/sd_module_key/
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)    30444 2024-04-23 14:19:45.000000 hidiffusion-0.1.5/hidiffusion/sd_module_key/sd15_module_key.txt
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)   100878 2024-04-23 14:19:45.000000 hidiffusion-0.1.5/hidiffusion/sd_module_key/sdxl_module_key.txt
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      872 2024-04-23 14:19:45.000000 hidiffusion-0.1.5/hidiffusion/utils.py
+drwxrwxr-x   0 zhangshen (10250) zhangshen (10250)        0 2024-04-23 14:21:35.217582 hidiffusion-0.1.5/hidiffusion.egg-info/
+-rw-r--r--   0 zhangshen (10250) zhangshen (10250)    15069 2024-04-23 14:21:35.000000 hidiffusion-0.1.5/hidiffusion.egg-info/PKG-INFO
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      334 2024-04-23 14:21:35.000000 hidiffusion-0.1.5/hidiffusion.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)        1 2024-04-23 14:21:35.000000 hidiffusion-0.1.5/hidiffusion.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)       12 2024-04-23 14:21:35.000000 hidiffusion-0.1.5/hidiffusion.egg-info/top_level.txt
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)       38 2024-04-23 14:21:35.217582 hidiffusion-0.1.5/setup.cfg
+-rw-rw-r--   0 zhangshen (10250) zhangshen (10250)      493 2024-04-23 14:20:54.000000 hidiffusion-0.1.5/setup.py
```

### Comparing `hidiffusion-0.1.4/PKG-INFO` & `hidiffusion-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: hidiffusion
-Version: 0.1.4
+Version: 0.1.5
 Summary: HiDiffusion: A training-free method to increase the resolution and speed of diffusion models.
 Home-page: 
 Author: Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang
 Description-Content-Type: text/markdown
 
 <!-- # 💡 HiDiffusion -->
 
+<div align="center">
+  <img src="assets/hidiffusion_logo.jpg"  height=120>
+</div>
+
 ### <div align="center">💡 HiDiffusion: Unlocking Higher-Resolution Creativity and Efficiency in Pretrained Diffusion Models</div> 
 
 <div align="center">Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang</div> 
 
 <br>
 
 <div align="center">
@@ -73,15 +77,15 @@
 After installing the packages in the [main requirements](#-main-requirements), install HiDiffusion:
 ```shell
 pip3 install hidiffusion
 ```
 ### Installing from source
 Alternatively, you can install from github source. Clone the repository and install:
 ```bash
-git clone https://github.com/ShenZhang-Shin/HiDiffusion.git
+git clone https://github.com/megvii-model/HiDiffusion.git
 cd HiDiffusion
 python3 setup.py install
 ```
 
 
 ## 🚀 Usage
 
@@ -256,23 +260,23 @@
 
 # Apply hidiffusion with a single line of code.
 apply_hidiffusion(pipe)
 
 pipe.enable_model_cpu_offload()
 pipe.enable_xformers_memory_efficient_attention()
 
-prompt = "a zombie, high face detail, high detail, muted color, 8k"
-negative_prompt = "blurry, ugly, duplicate, poorly drawn, deformed, mosaic, poorly drawn teeth, duplicated teeth."
+prompt = "The Joker, high face detail, high detail, muted color, 8k"
+negative_prompt = "blurry, ugly, duplicate, poorly drawn, deformed, mosaic."
 
 image = pipe(
     prompt, controlnet_conditioning_scale=controlnet_conditioning_scale, image=canny_image,
     height=2048, width=2048, guidance_scale=7.5, negative_prompt = negative_prompt, eta=1.0
 ).images[0]
 
-image.save('zombie.jpg')
+image.save('joker.jpg')
 ```
 
 <details>
 <summary>Output:</summary>
 <div align="center">
   <img src="assets/controlnet_result.jpg" width="800" ></img>
 </div>
@@ -347,14 +351,15 @@
 <summary>Output:</summary>
 <div align="center">
   <img src="assets/ghibli_diffusion.jpg" width="800" ></img>
 </div>
 </details>
 
 ### Playground
+
 ```python
 from diffusers import DiffusionPipeline
 import torch
 from hidiffusion import apply_hidiffusion, remove_hidiffusion
 
 pipe = DiffusionPipeline.from_pretrained(
     "playgroundai/playground-v2-1024px-aesthetic",
@@ -370,14 +375,17 @@
 apply_hidiffusion(pipe)
 
 prompt = "The little girl riding a bike, in a beautiful anime scene by Hayao Miyazaki: a snowy Tokyo city with massive Miyazaki clouds floating in the blue sky, enchanting snowscapes of the city with bright sunlight, Miyazaki's landscape imagery, Japanese art"
 negative_prompt="blurry, ugly, duplicate, poorly drawn, deformed, mosaic"
 image  = pipe(prompt=prompt, guidance_scale=3.0, height=2048, width=2048, negative_prompt=negative_prompt).images[0]
 image.save('girl.jpg')
 ```
+
+Note: You may change guidance scale from 3.0 to 5.0 and design appropriate negative prompt to generate satisfactory results.
+
 <details>
 <summary>Output:</summary>
 <div align="center">
   <img src="assets/playground_result.jpg" width="800" ></img>
 </div>
 </details>
```

#### html2text {}

```diff
@@ -1,11 +1,13 @@
-Metadata-Version: 2.1 Name: hidiffusion Version: 0.1.4 Summary: HiDiffusion: A
+Metadata-Version: 2.1 Name: hidiffusion Version: 0.1.5 Summary: HiDiffusion: A
 training-free method to increase the resolution and speed of diffusion models.
 Home-page: Author: Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang,
-Jiajun Liang Description-Content-Type: text/markdown ###
+Jiajun Liang Description-Content-Type: text/markdown
+                         [assets/hidiffusion_logo.jpg]
+###
   ð¡ HiDiffusion: Unlocking Higher-Resolution Creativity and Efficiency in
                           Pretrained Diffusion Models
    Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang
 
                         _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_s_t_a_t_i_c_/
 _v_1_?_l_a_b_e_l_=_P_r_o_j_e_c_t_%_2_0_P_a_g_e_&_m_e_s_s_a_g_e_=_G_i_t_h_u_b_&_c_o_l_o_r_=_b_l_u_e_&_l_o_g_o_=_g_i_t_h_u_b_-_p_a_g_e_s_]  _[_h_t_t_p_s_:_/_/
               _i_m_g_._s_h_i_e_l_d_s_._i_o_/_s_t_a_t_i_c_/_v_1_?_l_a_b_e_l_=_P_a_p_e_r_&_m_e_s_s_a_g_e_=_A_r_x_i_v_:
@@ -33,22 +35,22 @@
 aesthetic), etc. ## ð£ Supported Tasks - â Text-to-image - â ControlNet -
 â Inpainting ## ð Main Requirements This repository is tested on *
 Python==3.8 * torch==1.13.1 * diffusers==0.27.0 * transformers==4.27.4 *
 accelerate==0.18.0 * xformers==0.0.16rc425 ## ð Install HiDiffusion After
 installing the packages in the [main requirements](#-main-requirements),
 install HiDiffusion: ```shell pip3 install hidiffusion ``` ### Installing from
 source Alternatively, you can install from github source. Clone the repository
-and install: ```bash git clone https://github.com/ShenZhang-Shin/
-HiDiffusion.git cd HiDiffusion python3 setup.py install ``` ## ð Usage
-Generating outputs with HiDiffusion is super easy based on ð¤ [diffusers]
-(https://github.com/huggingface/diffusers/tree/main). **You just need to add a
-single line of code**. ## Text-to-image generation ### Stable Diffusion XL
-```python from hidiffusion import apply_hidiffusion, remove_hidiffusion from
-diffusers import StableDiffusionXLPipeline, DDIMScheduler import torch
-pretrain_model = "stabilityai/stable-diffusion-xl-base-1.0" scheduler =
+and install: ```bash git clone https://github.com/megvii-model/HiDiffusion.git
+cd HiDiffusion python3 setup.py install ``` ## ð Usage Generating outputs
+with HiDiffusion is super easy based on ð¤ [diffusers](https://github.com/
+huggingface/diffusers/tree/main). **You just need to add a single line of
+code**. ## Text-to-image generation ### Stable Diffusion XL ```python from
+hidiffusion import apply_hidiffusion, remove_hidiffusion from diffusers import
+StableDiffusionXLPipeline, DDIMScheduler import torch pretrain_model =
+"stabilityai/stable-diffusion-xl-base-1.0" scheduler =
 DDIMScheduler.from_pretrained(pretrain_model, subfolder="scheduler") pipe =
 StableDiffusionXLPipeline.from_pretrained(pretrain_model, scheduler =
 scheduler, torch_dtype=torch.float16, variant="fp16").to("cuda") # # Optional.
 enable_xformers_memory_efficient_attention can save memory usage and increase
 inference speed. enable_model_cpu_offload and enable_vae_tiling can save memory
 usage. # pipe.enable_xformers_memory_efficient_attention() #
 pipe.enable_model_cpu_offload() # pipe.enable_vae_tiling() # Apply hidiffusion
@@ -128,21 +130,20 @@
 1.0", torch_dtype=torch.float16, variant="fp16" ) scheduler =
 DDIMScheduler.from_pretrained("stabilityai/stable-diffusion-xl-base-1.0",
 subfolder="scheduler") pipe =
 StableDiffusionXLControlNetPipeline.from_pretrained( "stabilityai/stable-
 diffusion-xl-base-1.0", controlnet=controlnet, torch_dtype=torch.float16,
 scheduler = scheduler ) # Apply hidiffusion with a single line of code.
 apply_hidiffusion(pipe) pipe.enable_model_cpu_offload()
-pipe.enable_xformers_memory_efficient_attention() prompt = "a zombie, high face
-detail, high detail, muted color, 8k" negative_prompt = "blurry, ugly,
-duplicate, poorly drawn, deformed, mosaic, poorly drawn teeth, duplicated
-teeth." image = pipe( prompt,
+pipe.enable_xformers_memory_efficient_attention() prompt = "The Joker, high
+face detail, high detail, muted color, 8k" negative_prompt = "blurry, ugly,
+duplicate, poorly drawn, deformed, mosaic." image = pipe( prompt,
 controlnet_conditioning_scale=controlnet_conditioning_scale, image=canny_image,
 height=2048, width=2048, guidance_scale=7.5, negative_prompt = negative_prompt,
-eta=1.0 ).images[0] image.save('zombie.jpg') ``` Output:
+eta=1.0 ).images[0] image.save('joker.jpg') ``` Output:
                         [assets/controlnet_result.jpg]
 ## Inpainting ```python import torch from diffusers import
 AutoPipelineForInpainting, DDIMScheduler from diffusers.utils import load_image
 from hidiffusion import apply_hidiffusion, remove_hidiffusion from PIL import
 Image scheduler = DDIMScheduler.from_pretrained("stabilityai/stable-diffusion-
 xl-base-1.0", subfolder="scheduler") pipeline =
 AutoPipelineForInpainting.from_pretrained( "diffusers/stable-diffusion-xl-1.0-
@@ -185,15 +186,17 @@
 pipe.enable_xformers_memory_efficient_attention() # Apply hidiffusion with a
 single line of code. apply_hidiffusion(pipe) prompt = "The little girl riding a
 bike, in a beautiful anime scene by Hayao Miyazaki: a snowy Tokyo city with
 massive Miyazaki clouds floating in the blue sky, enchanting snowscapes of the
 city with bright sunlight, Miyazaki's landscape imagery, Japanese art"
 negative_prompt="blurry, ugly, duplicate, poorly drawn, deformed, mosaic" image
 = pipe(prompt=prompt, guidance_scale=3.0, height=2048, width=2048,
-negative_prompt=negative_prompt).images[0] image.save('girl.jpg') ``` Output:
+negative_prompt=negative_prompt).images[0] image.save('girl.jpg') ``` Note: You
+may change guidance scale from 3.0 to 5.0 and design appropriate negative
+prompt to generate satisfactory results. Output:
                         [assets/playground_result.jpg]
 ## ð Acknowledgements This codebase is based on [tomesd](https://github.com/
 dbolya/tomesd) and [diffusers](https://github.com/huggingface/diffusers/tree/
 main). Thanks! ## ð Citation ``` @article{zhang2023hidiffusion, title=
 {HiDiffusion: Unlocking Higher-Resolution Creativity and Efficiency in
 Pretrained Diffusion Models}, author={Zhang, Shen and Chen, Zhaowei and Zhao,
 Zhenyu and Chen, Yuhao and Tang, Yao and Liang, Jiajun}, journal={arXiv
```

### Comparing `hidiffusion-0.1.4/README.md` & `hidiffusion-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 <!-- # 💡 HiDiffusion -->
 
+<div align="center">
+  <img src="assets/hidiffusion_logo.jpg"  height=120>
+</div>
+
 ### <div align="center">💡 HiDiffusion: Unlocking Higher-Resolution Creativity and Efficiency in Pretrained Diffusion Models</div> 
 
 <div align="center">Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang</div> 
 
 <br>
 
 <div align="center">
@@ -65,15 +69,15 @@
 After installing the packages in the [main requirements](#-main-requirements), install HiDiffusion:
 ```shell
 pip3 install hidiffusion
 ```
 ### Installing from source
 Alternatively, you can install from github source. Clone the repository and install:
 ```bash
-git clone https://github.com/ShenZhang-Shin/HiDiffusion.git
+git clone https://github.com/megvii-model/HiDiffusion.git
 cd HiDiffusion
 python3 setup.py install
 ```
 
 
 ## 🚀 Usage
 
@@ -248,23 +252,23 @@
 
 # Apply hidiffusion with a single line of code.
 apply_hidiffusion(pipe)
 
 pipe.enable_model_cpu_offload()
 pipe.enable_xformers_memory_efficient_attention()
 
-prompt = "a zombie, high face detail, high detail, muted color, 8k"
-negative_prompt = "blurry, ugly, duplicate, poorly drawn, deformed, mosaic, poorly drawn teeth, duplicated teeth."
+prompt = "The Joker, high face detail, high detail, muted color, 8k"
+negative_prompt = "blurry, ugly, duplicate, poorly drawn, deformed, mosaic."
 
 image = pipe(
     prompt, controlnet_conditioning_scale=controlnet_conditioning_scale, image=canny_image,
     height=2048, width=2048, guidance_scale=7.5, negative_prompt = negative_prompt, eta=1.0
 ).images[0]
 
-image.save('zombie.jpg')
+image.save('joker.jpg')
 ```
 
 <details>
 <summary>Output:</summary>
 <div align="center">
   <img src="assets/controlnet_result.jpg" width="800" ></img>
 </div>
@@ -339,14 +343,15 @@
 <summary>Output:</summary>
 <div align="center">
   <img src="assets/ghibli_diffusion.jpg" width="800" ></img>
 </div>
 </details>
 
 ### Playground
+
 ```python
 from diffusers import DiffusionPipeline
 import torch
 from hidiffusion import apply_hidiffusion, remove_hidiffusion
 
 pipe = DiffusionPipeline.from_pretrained(
     "playgroundai/playground-v2-1024px-aesthetic",
@@ -362,14 +367,17 @@
 apply_hidiffusion(pipe)
 
 prompt = "The little girl riding a bike, in a beautiful anime scene by Hayao Miyazaki: a snowy Tokyo city with massive Miyazaki clouds floating in the blue sky, enchanting snowscapes of the city with bright sunlight, Miyazaki's landscape imagery, Japanese art"
 negative_prompt="blurry, ugly, duplicate, poorly drawn, deformed, mosaic"
 image  = pipe(prompt=prompt, guidance_scale=3.0, height=2048, width=2048, negative_prompt=negative_prompt).images[0]
 image.save('girl.jpg')
 ```
+
+Note: You may change guidance scale from 3.0 to 5.0 and design appropriate negative prompt to generate satisfactory results.
+
 <details>
 <summary>Output:</summary>
 <div align="center">
   <img src="assets/playground_result.jpg" width="800" ></img>
 </div>
 </details>
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
+                         [assets/hidiffusion_logo.jpg]
 ###
   ð¡ HiDiffusion: Unlocking Higher-Resolution Creativity and Efficiency in
                           Pretrained Diffusion Models
    Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang
 
                         _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_s_t_a_t_i_c_/
 _v_1_?_l_a_b_e_l_=_P_r_o_j_e_c_t_%_2_0_P_a_g_e_&_m_e_s_s_a_g_e_=_G_i_t_h_u_b_&_c_o_l_o_r_=_b_l_u_e_&_l_o_g_o_=_g_i_t_h_u_b_-_p_a_g_e_s_]  _[_h_t_t_p_s_:_/_/
@@ -30,22 +31,22 @@
 aesthetic), etc. ## ð£ Supported Tasks - â Text-to-image - â ControlNet -
 â Inpainting ## ð Main Requirements This repository is tested on *
 Python==3.8 * torch==1.13.1 * diffusers==0.27.0 * transformers==4.27.4 *
 accelerate==0.18.0 * xformers==0.0.16rc425 ## ð Install HiDiffusion After
 installing the packages in the [main requirements](#-main-requirements),
 install HiDiffusion: ```shell pip3 install hidiffusion ``` ### Installing from
 source Alternatively, you can install from github source. Clone the repository
-and install: ```bash git clone https://github.com/ShenZhang-Shin/
-HiDiffusion.git cd HiDiffusion python3 setup.py install ``` ## ð Usage
-Generating outputs with HiDiffusion is super easy based on ð¤ [diffusers]
-(https://github.com/huggingface/diffusers/tree/main). **You just need to add a
-single line of code**. ## Text-to-image generation ### Stable Diffusion XL
-```python from hidiffusion import apply_hidiffusion, remove_hidiffusion from
-diffusers import StableDiffusionXLPipeline, DDIMScheduler import torch
-pretrain_model = "stabilityai/stable-diffusion-xl-base-1.0" scheduler =
+and install: ```bash git clone https://github.com/megvii-model/HiDiffusion.git
+cd HiDiffusion python3 setup.py install ``` ## ð Usage Generating outputs
+with HiDiffusion is super easy based on ð¤ [diffusers](https://github.com/
+huggingface/diffusers/tree/main). **You just need to add a single line of
+code**. ## Text-to-image generation ### Stable Diffusion XL ```python from
+hidiffusion import apply_hidiffusion, remove_hidiffusion from diffusers import
+StableDiffusionXLPipeline, DDIMScheduler import torch pretrain_model =
+"stabilityai/stable-diffusion-xl-base-1.0" scheduler =
 DDIMScheduler.from_pretrained(pretrain_model, subfolder="scheduler") pipe =
 StableDiffusionXLPipeline.from_pretrained(pretrain_model, scheduler =
 scheduler, torch_dtype=torch.float16, variant="fp16").to("cuda") # # Optional.
 enable_xformers_memory_efficient_attention can save memory usage and increase
 inference speed. enable_model_cpu_offload and enable_vae_tiling can save memory
 usage. # pipe.enable_xformers_memory_efficient_attention() #
 pipe.enable_model_cpu_offload() # pipe.enable_vae_tiling() # Apply hidiffusion
@@ -125,21 +126,20 @@
 1.0", torch_dtype=torch.float16, variant="fp16" ) scheduler =
 DDIMScheduler.from_pretrained("stabilityai/stable-diffusion-xl-base-1.0",
 subfolder="scheduler") pipe =
 StableDiffusionXLControlNetPipeline.from_pretrained( "stabilityai/stable-
 diffusion-xl-base-1.0", controlnet=controlnet, torch_dtype=torch.float16,
 scheduler = scheduler ) # Apply hidiffusion with a single line of code.
 apply_hidiffusion(pipe) pipe.enable_model_cpu_offload()
-pipe.enable_xformers_memory_efficient_attention() prompt = "a zombie, high face
-detail, high detail, muted color, 8k" negative_prompt = "blurry, ugly,
-duplicate, poorly drawn, deformed, mosaic, poorly drawn teeth, duplicated
-teeth." image = pipe( prompt,
+pipe.enable_xformers_memory_efficient_attention() prompt = "The Joker, high
+face detail, high detail, muted color, 8k" negative_prompt = "blurry, ugly,
+duplicate, poorly drawn, deformed, mosaic." image = pipe( prompt,
 controlnet_conditioning_scale=controlnet_conditioning_scale, image=canny_image,
 height=2048, width=2048, guidance_scale=7.5, negative_prompt = negative_prompt,
-eta=1.0 ).images[0] image.save('zombie.jpg') ``` Output:
+eta=1.0 ).images[0] image.save('joker.jpg') ``` Output:
                         [assets/controlnet_result.jpg]
 ## Inpainting ```python import torch from diffusers import
 AutoPipelineForInpainting, DDIMScheduler from diffusers.utils import load_image
 from hidiffusion import apply_hidiffusion, remove_hidiffusion from PIL import
 Image scheduler = DDIMScheduler.from_pretrained("stabilityai/stable-diffusion-
 xl-base-1.0", subfolder="scheduler") pipeline =
 AutoPipelineForInpainting.from_pretrained( "diffusers/stable-diffusion-xl-1.0-
@@ -182,15 +182,17 @@
 pipe.enable_xformers_memory_efficient_attention() # Apply hidiffusion with a
 single line of code. apply_hidiffusion(pipe) prompt = "The little girl riding a
 bike, in a beautiful anime scene by Hayao Miyazaki: a snowy Tokyo city with
 massive Miyazaki clouds floating in the blue sky, enchanting snowscapes of the
 city with bright sunlight, Miyazaki's landscape imagery, Japanese art"
 negative_prompt="blurry, ugly, duplicate, poorly drawn, deformed, mosaic" image
 = pipe(prompt=prompt, guidance_scale=3.0, height=2048, width=2048,
-negative_prompt=negative_prompt).images[0] image.save('girl.jpg') ``` Output:
+negative_prompt=negative_prompt).images[0] image.save('girl.jpg') ``` Note: You
+may change guidance scale from 3.0 to 5.0 and design appropriate negative
+prompt to generate satisfactory results. Output:
                         [assets/playground_result.jpg]
 ## ð Acknowledgements This codebase is based on [tomesd](https://github.com/
 dbolya/tomesd) and [diffusers](https://github.com/huggingface/diffusers/tree/
 main). Thanks! ## ð Citation ``` @article{zhang2023hidiffusion, title=
 {HiDiffusion: Unlocking Higher-Resolution Creativity and Efficiency in
 Pretrained Diffusion Models}, author={Zhang, Shen and Chen, Zhaowei and Zhao,
 Zhenyu and Chen, Yuhao and Tang, Yao and Liang, Jiajun}, journal={arXiv
```

### Comparing `hidiffusion-0.1.4/hidiffusion/hidiffusion.py` & `hidiffusion-0.1.5/hidiffusion/hidiffusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 }
 controlnet_apply_steps_rate = 0.6
 
 is_aggressive_raunet = True
 aggressive_step = 8
 
 inpainting_is_aggressive_raunet = False
+playground_is_aggressive_raunet = False
 
 current_path = os.path.dirname(__file__)
 module_key_path = os.path.join(current_path, "sd_module_key")
 with open(os.path.join(module_key_path, 'sd15_module_key.txt'), 'r') as f:
     sd15_module_key = f.read().splitlines()
     
 with open(os.path.join(module_key_path, 'sdxl_module_key.txt'), 'r') as f:
@@ -357,30 +358,50 @@
                 mult = len(controlnet.nets) if isinstance(controlnet, MultiControlNetModel) else 1
                 control_guidance_start, control_guidance_end = (
                     mult * [control_guidance_start],
                     mult * [control_guidance_end],
                 )
 
             # 1. Check inputs. Raise error if not correct
-            self.check_inputs(
-                prompt,
-                prompt_2,
-                image,
-                callback_steps,
-                negative_prompt,
-                negative_prompt_2,
-                prompt_embeds,
-                negative_prompt_embeds,
-                pooled_prompt_embeds,
-                negative_pooled_prompt_embeds,
-                controlnet_conditioning_scale,
-                control_guidance_start,
-                control_guidance_end,
-                callback_on_step_end_tensor_inputs,
-            )
+            if old_diffusers:
+                self.check_inputs(
+                    prompt,
+                    prompt_2,
+                    image,
+                    callback_steps,
+                    negative_prompt,
+                    negative_prompt_2,
+                    prompt_embeds,
+                    negative_prompt_embeds,
+                    pooled_prompt_embeds,
+                    negative_pooled_prompt_embeds,
+                    controlnet_conditioning_scale,
+                    control_guidance_start,
+                    control_guidance_end,
+                    callback_on_step_end_tensor_inputs,
+                )
+            else:
+                self.check_inputs(
+                    prompt,
+                    prompt_2,
+                    image,
+                    callback_steps,
+                    negative_prompt,
+                    negative_prompt_2,
+                    prompt_embeds,
+                    negative_prompt_embeds,
+                    pooled_prompt_embeds,
+                    None,
+                    None,
+                    negative_pooled_prompt_embeds,
+                    controlnet_conditioning_scale,
+                    control_guidance_start,
+                    control_guidance_end,
+                    callback_on_step_end_tensor_inputs,
+                )
 
             self._guidance_scale = guidance_scale
             self._clip_skip = clip_skip
             self._cross_attention_kwargs = cross_attention_kwargs
 
             # 2. Define call parameters
             if prompt is not None and isinstance(prompt, str):
@@ -1353,14 +1374,16 @@
                     if self.info['use_controlnet']:
                         self.T1_ratio = controlnet_switching_threshold_ratio_dict['sdxl_2048'][self.switching_threshold_ratio]
                     else:
                         self.T1_ratio = switching_threshold_ratio_dict['sdxl_2048'][self.switching_threshold_ratio]
                         
                     if self.info['is_inpainting_task']:
                         self.aggressive_raunet = inpainting_is_aggressive_raunet
+                    elif self.info['is_playground']:
+                        self.aggressive_raunet = playground_is_aggressive_raunet
                     else:
                         self.aggressive_raunet = is_aggressive_raunet
                 else:
                     self.T1_ratio = switching_threshold_ratio_dict['sdxl_4096'][self.switching_threshold_ratio]
             elif self.model == 'sdxl_turbo':
                 self.T1_ratio = switching_threshold_ratio_dict['sdxl_turbo_1024'][self.switching_threshold_ratio]
             else:
@@ -1478,18 +1501,22 @@
                     self.T1_ratio = switching_threshold_ratio_dict['sd15_2048'][self.switching_threshold_ratio]
             elif self.model == 'sdxl':
                 if ori_H < 512 or ori_W < 512:
                     if self.info['use_controlnet']:
                         self.T1_ratio = controlnet_switching_threshold_ratio_dict['sdxl_2048'][self.switching_threshold_ratio]
                     else:
                         self.T1_ratio = switching_threshold_ratio_dict['sdxl_2048'][self.switching_threshold_ratio]
+                        
                     if self.info['is_inpainting_task']:
                         self.aggressive_raunet = inpainting_is_aggressive_raunet
+                    elif self.info['is_playground']:
+                        self.aggressive_raunet = playground_is_aggressive_raunet
                     else:
                         self.aggressive_raunet = is_aggressive_raunet
+                        
                 else:
                     self.T1_ratio = switching_threshold_ratio_dict['sdxl_4096'][self.switching_threshold_ratio]
             elif self.model == 'sdxl_turbo':
                 self.T1_ratio = switching_threshold_ratio_dict['sdxl_turbo_1024'][self.switching_threshold_ratio]
             else:
                 raise Exception(f'Error model. HiDiffusion now only supports sd15, sd21, sdxl, sdxl-turbo.') 
             
@@ -1609,16 +1636,19 @@
                     self.T1_ratio = switching_threshold_ratio_dict['sd15_2048'][self.switching_threshold_ratio]
             elif self.model == 'sdxl':
                 if ori_H < 512 or ori_W < 512:
                     if self.info['use_controlnet']:
                         self.T1_ratio = controlnet_switching_threshold_ratio_dict['sdxl_2048'][self.switching_threshold_ratio]
                     else:
                         self.T1_ratio = switching_threshold_ratio_dict['sdxl_2048'][self.switching_threshold_ratio]
+                        
                     if self.info['is_inpainting_task']:
                         self.aggressive_raunet = inpainting_is_aggressive_raunet
+                    elif self.info['is_playground']:
+                        self.aggressive_raunet = playground_is_aggressive_raunet
                     else:
                         self.aggressive_raunet = is_aggressive_raunet
                 else:
                     self.T1_ratio = switching_threshold_ratio_dict['sdxl_4096'][self.switching_threshold_ratio]
             elif self.model == 'sdxl_turbo':
                 self.T1_ratio = switching_threshold_ratio_dict['sdxl_turbo_1024'][self.switching_threshold_ratio]
             else:
@@ -1695,16 +1725,19 @@
                     self.T1_ratio = switching_threshold_ratio_dict['sd15_2048'][self.switching_threshold_ratio]
             elif self.model == 'sdxl':
                 if ori_H < 512 or ori_W < 512:
                     if self.info['use_controlnet']:
                         self.T1_ratio = controlnet_switching_threshold_ratio_dict['sdxl_2048'][self.switching_threshold_ratio]
                     else:
                         self.T1_ratio = switching_threshold_ratio_dict['sdxl_2048'][self.switching_threshold_ratio]
+                        
                     if self.info['is_inpainting_task']:
                         self.aggressive_raunet = inpainting_is_aggressive_raunet
+                    elif self.info['is_playground']:
+                        self.aggressive_raunet = playground_is_aggressive_raunet
                     else:
                         self.aggressive_raunet = is_aggressive_raunet
                 else:
                     self.T1_ratio = switching_threshold_ratio_dict['sdxl_4096'][self.switching_threshold_ratio]
             elif self.model == 'sdxl_turbo':
                 self.T1_ratio = switching_threshold_ratio_dict['sdxl_turbo_1024'][self.switching_threshold_ratio]
             else:
@@ -1791,17 +1824,16 @@
         for key, module in diffusion_model.named_modules():
             diffusion_model_module_key.append(key)
         if set(sd15_module_key) < set(diffusion_model_module_key):
             name_or_path = 'runwayml/stable-diffusion-v1-5'
         elif set(sdxl_module_key) < set(diffusion_model_module_key):
             name_or_path = 'stabilityai/stable-diffusion-xl-base-1.0'
 
-        
     diffusion_model.info = {'size': None, 'hooks': [], 'scheduler': model.scheduler, 'use_controlnet': hasattr(model, 'controlnet'),
-                            'is_inpainting_task': 'inpainting' in model.name_or_path}
+                            'is_inpainting_task': 'inpainting' in model.name_or_path, 'is_playground': 'playground' in model.name_or_path}
     hook_diffusion_model(diffusion_model)
     
     if name_or_path in ['runwayml/stable-diffusion-v1-5', 'stabilityai/stable-diffusion-2-1-base']:
         modified_key = sd15_hidiffusion_key()
         for key, module in diffusion_model.named_modules():
             if apply_raunet and key in modified_key['down_module_key']:
                 make_block_fn = make_diffusers_downsampler_block
```

### Comparing `hidiffusion-0.1.4/hidiffusion/sd_module_key/sd15_module_key.txt` & `hidiffusion-0.1.5/hidiffusion/sd_module_key/sd15_module_key.txt`

 * *Files identical despite different names*

### Comparing `hidiffusion-0.1.4/hidiffusion/sd_module_key/sdxl_module_key.txt` & `hidiffusion-0.1.5/hidiffusion/sd_module_key/sdxl_module_key.txt`

 * *Files identical despite different names*

### Comparing `hidiffusion-0.1.4/hidiffusion/utils.py` & `hidiffusion-0.1.5/hidiffusion/utils.py`

 * *Files identical despite different names*

### Comparing `hidiffusion-0.1.4/hidiffusion.egg-info/PKG-INFO` & `hidiffusion-0.1.5/hidiffusion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: hidiffusion
-Version: 0.1.4
+Version: 0.1.5
 Summary: HiDiffusion: A training-free method to increase the resolution and speed of diffusion models.
 Home-page: 
 Author: Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang
 Description-Content-Type: text/markdown
 
 <!-- # 💡 HiDiffusion -->
 
+<div align="center">
+  <img src="assets/hidiffusion_logo.jpg"  height=120>
+</div>
+
 ### <div align="center">💡 HiDiffusion: Unlocking Higher-Resolution Creativity and Efficiency in Pretrained Diffusion Models</div> 
 
 <div align="center">Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang</div> 
 
 <br>
 
 <div align="center">
@@ -73,15 +77,15 @@
 After installing the packages in the [main requirements](#-main-requirements), install HiDiffusion:
 ```shell
 pip3 install hidiffusion
 ```
 ### Installing from source
 Alternatively, you can install from github source. Clone the repository and install:
 ```bash
-git clone https://github.com/ShenZhang-Shin/HiDiffusion.git
+git clone https://github.com/megvii-model/HiDiffusion.git
 cd HiDiffusion
 python3 setup.py install
 ```
 
 
 ## 🚀 Usage
 
@@ -256,23 +260,23 @@
 
 # Apply hidiffusion with a single line of code.
 apply_hidiffusion(pipe)
 
 pipe.enable_model_cpu_offload()
 pipe.enable_xformers_memory_efficient_attention()
 
-prompt = "a zombie, high face detail, high detail, muted color, 8k"
-negative_prompt = "blurry, ugly, duplicate, poorly drawn, deformed, mosaic, poorly drawn teeth, duplicated teeth."
+prompt = "The Joker, high face detail, high detail, muted color, 8k"
+negative_prompt = "blurry, ugly, duplicate, poorly drawn, deformed, mosaic."
 
 image = pipe(
     prompt, controlnet_conditioning_scale=controlnet_conditioning_scale, image=canny_image,
     height=2048, width=2048, guidance_scale=7.5, negative_prompt = negative_prompt, eta=1.0
 ).images[0]
 
-image.save('zombie.jpg')
+image.save('joker.jpg')
 ```
 
 <details>
 <summary>Output:</summary>
 <div align="center">
   <img src="assets/controlnet_result.jpg" width="800" ></img>
 </div>
@@ -347,14 +351,15 @@
 <summary>Output:</summary>
 <div align="center">
   <img src="assets/ghibli_diffusion.jpg" width="800" ></img>
 </div>
 </details>
 
 ### Playground
+
 ```python
 from diffusers import DiffusionPipeline
 import torch
 from hidiffusion import apply_hidiffusion, remove_hidiffusion
 
 pipe = DiffusionPipeline.from_pretrained(
     "playgroundai/playground-v2-1024px-aesthetic",
@@ -370,14 +375,17 @@
 apply_hidiffusion(pipe)
 
 prompt = "The little girl riding a bike, in a beautiful anime scene by Hayao Miyazaki: a snowy Tokyo city with massive Miyazaki clouds floating in the blue sky, enchanting snowscapes of the city with bright sunlight, Miyazaki's landscape imagery, Japanese art"
 negative_prompt="blurry, ugly, duplicate, poorly drawn, deformed, mosaic"
 image  = pipe(prompt=prompt, guidance_scale=3.0, height=2048, width=2048, negative_prompt=negative_prompt).images[0]
 image.save('girl.jpg')
 ```
+
+Note: You may change guidance scale from 3.0 to 5.0 and design appropriate negative prompt to generate satisfactory results.
+
 <details>
 <summary>Output:</summary>
 <div align="center">
   <img src="assets/playground_result.jpg" width="800" ></img>
 </div>
 </details>
```

#### html2text {}

```diff
@@ -1,11 +1,13 @@
-Metadata-Version: 2.1 Name: hidiffusion Version: 0.1.4 Summary: HiDiffusion: A
+Metadata-Version: 2.1 Name: hidiffusion Version: 0.1.5 Summary: HiDiffusion: A
 training-free method to increase the resolution and speed of diffusion models.
 Home-page: Author: Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang,
-Jiajun Liang Description-Content-Type: text/markdown ###
+Jiajun Liang Description-Content-Type: text/markdown
+                         [assets/hidiffusion_logo.jpg]
+###
   ð¡ HiDiffusion: Unlocking Higher-Resolution Creativity and Efficiency in
                           Pretrained Diffusion Models
    Shen Zhang, Zhaowei Chen, Zhenyu Zhao, Yuhao Chen, Yao Tang, Jiajun Liang
 
                         _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_s_t_a_t_i_c_/
 _v_1_?_l_a_b_e_l_=_P_r_o_j_e_c_t_%_2_0_P_a_g_e_&_m_e_s_s_a_g_e_=_G_i_t_h_u_b_&_c_o_l_o_r_=_b_l_u_e_&_l_o_g_o_=_g_i_t_h_u_b_-_p_a_g_e_s_]  _[_h_t_t_p_s_:_/_/
               _i_m_g_._s_h_i_e_l_d_s_._i_o_/_s_t_a_t_i_c_/_v_1_?_l_a_b_e_l_=_P_a_p_e_r_&_m_e_s_s_a_g_e_=_A_r_x_i_v_:
@@ -33,22 +35,22 @@
 aesthetic), etc. ## ð£ Supported Tasks - â Text-to-image - â ControlNet -
 â Inpainting ## ð Main Requirements This repository is tested on *
 Python==3.8 * torch==1.13.1 * diffusers==0.27.0 * transformers==4.27.4 *
 accelerate==0.18.0 * xformers==0.0.16rc425 ## ð Install HiDiffusion After
 installing the packages in the [main requirements](#-main-requirements),
 install HiDiffusion: ```shell pip3 install hidiffusion ``` ### Installing from
 source Alternatively, you can install from github source. Clone the repository
-and install: ```bash git clone https://github.com/ShenZhang-Shin/
-HiDiffusion.git cd HiDiffusion python3 setup.py install ``` ## ð Usage
-Generating outputs with HiDiffusion is super easy based on ð¤ [diffusers]
-(https://github.com/huggingface/diffusers/tree/main). **You just need to add a
-single line of code**. ## Text-to-image generation ### Stable Diffusion XL
-```python from hidiffusion import apply_hidiffusion, remove_hidiffusion from
-diffusers import StableDiffusionXLPipeline, DDIMScheduler import torch
-pretrain_model = "stabilityai/stable-diffusion-xl-base-1.0" scheduler =
+and install: ```bash git clone https://github.com/megvii-model/HiDiffusion.git
+cd HiDiffusion python3 setup.py install ``` ## ð Usage Generating outputs
+with HiDiffusion is super easy based on ð¤ [diffusers](https://github.com/
+huggingface/diffusers/tree/main). **You just need to add a single line of
+code**. ## Text-to-image generation ### Stable Diffusion XL ```python from
+hidiffusion import apply_hidiffusion, remove_hidiffusion from diffusers import
+StableDiffusionXLPipeline, DDIMScheduler import torch pretrain_model =
+"stabilityai/stable-diffusion-xl-base-1.0" scheduler =
 DDIMScheduler.from_pretrained(pretrain_model, subfolder="scheduler") pipe =
 StableDiffusionXLPipeline.from_pretrained(pretrain_model, scheduler =
 scheduler, torch_dtype=torch.float16, variant="fp16").to("cuda") # # Optional.
 enable_xformers_memory_efficient_attention can save memory usage and increase
 inference speed. enable_model_cpu_offload and enable_vae_tiling can save memory
 usage. # pipe.enable_xformers_memory_efficient_attention() #
 pipe.enable_model_cpu_offload() # pipe.enable_vae_tiling() # Apply hidiffusion
@@ -128,21 +130,20 @@
 1.0", torch_dtype=torch.float16, variant="fp16" ) scheduler =
 DDIMScheduler.from_pretrained("stabilityai/stable-diffusion-xl-base-1.0",
 subfolder="scheduler") pipe =
 StableDiffusionXLControlNetPipeline.from_pretrained( "stabilityai/stable-
 diffusion-xl-base-1.0", controlnet=controlnet, torch_dtype=torch.float16,
 scheduler = scheduler ) # Apply hidiffusion with a single line of code.
 apply_hidiffusion(pipe) pipe.enable_model_cpu_offload()
-pipe.enable_xformers_memory_efficient_attention() prompt = "a zombie, high face
-detail, high detail, muted color, 8k" negative_prompt = "blurry, ugly,
-duplicate, poorly drawn, deformed, mosaic, poorly drawn teeth, duplicated
-teeth." image = pipe( prompt,
+pipe.enable_xformers_memory_efficient_attention() prompt = "The Joker, high
+face detail, high detail, muted color, 8k" negative_prompt = "blurry, ugly,
+duplicate, poorly drawn, deformed, mosaic." image = pipe( prompt,
 controlnet_conditioning_scale=controlnet_conditioning_scale, image=canny_image,
 height=2048, width=2048, guidance_scale=7.5, negative_prompt = negative_prompt,
-eta=1.0 ).images[0] image.save('zombie.jpg') ``` Output:
+eta=1.0 ).images[0] image.save('joker.jpg') ``` Output:
                         [assets/controlnet_result.jpg]
 ## Inpainting ```python import torch from diffusers import
 AutoPipelineForInpainting, DDIMScheduler from diffusers.utils import load_image
 from hidiffusion import apply_hidiffusion, remove_hidiffusion from PIL import
 Image scheduler = DDIMScheduler.from_pretrained("stabilityai/stable-diffusion-
 xl-base-1.0", subfolder="scheduler") pipeline =
 AutoPipelineForInpainting.from_pretrained( "diffusers/stable-diffusion-xl-1.0-
@@ -185,15 +186,17 @@
 pipe.enable_xformers_memory_efficient_attention() # Apply hidiffusion with a
 single line of code. apply_hidiffusion(pipe) prompt = "The little girl riding a
 bike, in a beautiful anime scene by Hayao Miyazaki: a snowy Tokyo city with
 massive Miyazaki clouds floating in the blue sky, enchanting snowscapes of the
 city with bright sunlight, Miyazaki's landscape imagery, Japanese art"
 negative_prompt="blurry, ugly, duplicate, poorly drawn, deformed, mosaic" image
 = pipe(prompt=prompt, guidance_scale=3.0, height=2048, width=2048,
-negative_prompt=negative_prompt).images[0] image.save('girl.jpg') ``` Output:
+negative_prompt=negative_prompt).images[0] image.save('girl.jpg') ``` Note: You
+may change guidance scale from 3.0 to 5.0 and design appropriate negative
+prompt to generate satisfactory results. Output:
                         [assets/playground_result.jpg]
 ## ð Acknowledgements This codebase is based on [tomesd](https://github.com/
 dbolya/tomesd) and [diffusers](https://github.com/huggingface/diffusers/tree/
 main). Thanks! ## ð Citation ``` @article{zhang2023hidiffusion, title=
 {HiDiffusion: Unlocking Higher-Resolution Creativity and Efficiency in
 Pretrained Diffusion Models}, author={Zhang, Shen and Chen, Zhaowei and Zhao,
 Zhenyu and Chen, Yuhao and Tang, Yao and Liang, Jiajun}, journal={arXiv
```

