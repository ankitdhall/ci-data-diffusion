# SGLang-Diffusion Nightly Performance Dashboard

*Generated: Oct 05 | Commit: `a977e3b`*

*Methodology `client-e2e-v1`: client-side latency through each framework's public API, from submit until the output is downloaded; 1 identical client warmup request(s) per case, discarded. First request = the first request after the server reports ready. Server perf dumps are telemetry only.*

*Excluded 27 historical run(s) from baselines and trends because their measurement methodology or warmup count differs. Missing metadata is not treated as matching explicit metadata.*

## SGLang-Diffusion Performance

| Model | Risk | Client samples | Server samples | First request (s) | sglang median (s) |
|-------|------|----------------|----------------|-------------------|---------|
| Anima-Base-v1.0-Diffusers | ✅ | 3 | 3/3 | 3.37 | **3.25** |
| FLUX.1-dev | ✅ | 3 | 3/3 | 4.43 | **4.44** |
| FLUX.2-dev | ✅ | 3 | 3/3 | 13.18 | **13.05** |
| Qwen-Image-2512 | ✅ | 3 | 3/3 | 8.35 | **8.35** |
| Qwen-Image-Edit-2511 | ✅ | 3 | 3/3 | 16.20 | **14.81** |
| Z-Image-Turbo | ✅ | 3 | 3/3 | 0.77 | **0.76** |
| Wan2.2-T2V-A14B-Diffusers | ✅ | 3 | 3/3 | 212.44 | **206.51** |
| Wan2.2-TI2V-5B-Diffusers | ✅ | 3 | 3/3 | 56.57 | **55.51** |
| LTX-2.3 | ✅ | 3 | 3/3 | 14.97 | **13.53** |
| ideogram-4-fp8 | ✅ | 3 | 3/3 | 3.85 | **3.81** |
| Cosmos3-Super | ✅ | 3 | 3/3 | 119.30 | **118.43** |
| Wan2.2-I2V-A14B-Diffusers | ✅ | 3 | 3/3 | 200.85 | **200.87** |
| MiniMax-H3 | ✅ | 3 | 3/3 | 76.81 | **77.07** |

## SGLang Server-Side Breakdown

| Model | Server total (s) | Text encode (s) | Denoise (s) | Decode (s) | Median denoise step (ms) |
|-------|------------------|-----------------|--------------|------------|---------------------------|
| Anima-Base-v1.0-Diffusers | 3.22 | 0.02 | 2.98 | 0.21 | 100.02 |
| FLUX.1-dev | 4.28 | 0.03 | 4.08 | 0.02 | 82.18 |
| FLUX.2-dev | 12.93 | 0.37 | 12.11 | 0.01 | 241.46 |
| Qwen-Image-2512 | 8.28 | 0.23 | 7.98 | 0.06 | 160.34 |
| Qwen-Image-Edit-2511 | 14.73 | N/A | 13.99 | 0.10 | 351.99 |
| Z-Image-Turbo | 0.63 | 0.13 | 0.49 | 0.01 | 56.71 |
| Wan2.2-T2V-A14B-Diffusers | 206.03 | 0.27 | 203.34 | 2.15 | 5086.18 |
| Wan2.2-TI2V-5B-Diffusers | 53.87 | 0.34 | 47.93 | 5.56 | 967.47 |
| LTX-2.3 | 12.01 | 0.40 | 8.63 | 0.98 | 283.79 |
| ideogram-4-fp8 | 3.71 | 0.13 | 3.49 | 0.08 | 177.55 |
| Cosmos3-Super | 117.88 | 0.00 | 114.78 | 2.38 | N/A |
| Wan2.2-I2V-A14B-Diffusers | 200.47 | 0.27 | 194.84 | 2.07 | 4868.06 |
| MiniMax-H3 | 76.52 | 0.05 | 73.92 | 1.18 | 1533.49 |

### Latency Trend: anima_base_t2i_1024

![Latency Trend anima_base_t2i_1024](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_anima_base_t2i_1024.png)


### Latency Trend: flux1_dev_t2i_1024

![Latency Trend flux1_dev_t2i_1024](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_flux1_dev_t2i_1024.png)


### Latency Trend: flux2_dev_t2i_1024

![Latency Trend flux2_dev_t2i_1024](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_flux2_dev_t2i_1024.png)


### Latency Trend: qwen_image_2512_t2i_1024

![Latency Trend qwen_image_2512_t2i_1024](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_qwen_image_2512_t2i_1024.png)


### Latency Trend: qwen_image_edit_2511

![Latency Trend qwen_image_edit_2511](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_qwen_image_edit_2511.png)


### Latency Trend: zimage_turbo_t2i_1024

![Latency Trend zimage_turbo_t2i_1024](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_zimage_turbo_t2i_1024.png)


### Latency Trend: wan22_t2v_a14b_720p

![Latency Trend wan22_t2v_a14b_720p](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_wan22_t2v_a14b_720p.png)


### Latency Trend: wan22_ti2v_5b_720p

![Latency Trend wan22_ti2v_5b_720p](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_wan22_ti2v_5b_720p.png)


### Latency Trend: ltx2.3_twostage_ti2v_2gpus

![Latency Trend ltx2.3_twostage_ti2v_2gpus](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_ltx2.3_twostage_ti2v_2gpus.png)


### Latency Trend: ideogram4_fp8_t2i_2gpu

![Latency Trend ideogram4_fp8_t2i_2gpu](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_ideogram4_fp8_t2i_2gpu.png)


### Latency Trend: cosmos3_super_t2v_2gpu

![Latency Trend cosmos3_super_t2v_2gpu](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_cosmos3_super_t2v_2gpu.png)


### Latency Trend: wan22_i2v_a14b_720p

![Latency Trend wan22_i2v_a14b_720p](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_wan22_i2v_a14b_720p.png)


### Latency Trend: minimax_h3_t2va_5s

![Latency Trend minimax_h3_t2va_5s](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_minimax_h3_t2va_5s.png)


## SGLang Performance Trend (Last 3 Runs)

| Date | Commit | anima_base_t2i_1024 (s) | flux1_dev_t2i_1024 (s) | flux2_dev_t2i_1024 (s) | qwen_image_2512_t2i_1024 (s) | qwen_image_edit_2511 (s) | zimage_turbo_t2i_1024 (s) | wan22_t2v_a14b_720p (s) | wan22_ti2v_5b_720p (s) | ltx2.3_twostage_ti2v_2gpus (s) | ideogram4_fp8_t2i_2gpu (s) | cosmos3_super_t2v_2gpu (s) | wan22_i2v_a14b_720p (s) | minimax_h3_t2va_5s (s) | Trend |
|------|--------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|-------|
| Oct 05 | `a977e3b` | 3.25 | 4.44 | 13.05 | 8.35 | 14.81 | 0.76 | 206.51 | 55.51 | 13.53 | 3.81 | 118.43 | 200.87 | 77.07 | :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Oct 03 | `5b5d721` | 3.26 | 4.47 | 13.02 | 8.37 | 14.83 | 0.76 | 206.80 | 54.51 | 14.73 | 3.81 | 118.51 | 201.10 | 77.44 | :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Oct 01 | `41cbe65` | 3.31 | 4.46 | 13.12 | 9.02 | 14.92 | 0.77 | 207.96 | 55.06 | 17.30 | 3.83 | 119.24 | 201.70 | 77.45 | -- |

---
*Generated by `generate_diffusion_dashboard.py` in SGLang nightly CI.*
