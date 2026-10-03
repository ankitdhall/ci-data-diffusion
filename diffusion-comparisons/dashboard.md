# SGLang-Diffusion Nightly Performance Dashboard

*Generated: Oct 03 | Commit: `5b5d721`*

*Methodology `client-e2e-v1`: client-side latency through each framework's public API, from submit until the output is downloaded; 1 identical client warmup request(s) per case, discarded. First request = the first request after the server reports ready. Server perf dumps are telemetry only.*

> [!WARNING]
> **Performance Regression Detected**
>
> - **zimage_turbo_t2i_1024** (sglang): 0.76s vs 4-run median 0.71s (+7.3%)


## SGLang-Diffusion Performance

| Model | Risk | Client samples | Server samples | First request (s) | sglang median (s) |
|-------|------|----------------|----------------|-------------------|---------|
| Anima-Base-v1.0-Diffusers | ✅ | 3 | 3/3 | 3.42 | **3.26** |
| FLUX.1-dev | ✅ | 3 | 3/3 | 4.44 | **4.47** |
| FLUX.2-dev | ✅ | 3 | 3/3 | 13.18 | **13.02** |
| Qwen-Image-2512 | ✅ | 3 | 3/3 | 8.38 | **8.37** |
| Qwen-Image-Edit-2511 | ✅ | 3 | 3/3 | 14.92 | **14.83** |
| Z-Image-Turbo | ⚠️ | 3 | 3/3 | 0.80 | **0.76** |
| Wan2.2-T2V-A14B-Diffusers | ✅ | 3 | 3/3 | 206.60 | **206.80** |
| Wan2.2-TI2V-5B-Diffusers | ✅ | 3 | 3/3 | 54.61 | **54.51** |
| LTX-2.3 | ✅ | 3 | 3/3 | 16.37 | **14.73** |
| ideogram-4-fp8 | ✅ | 3 | 3/3 | 3.92 | **3.81** |
| Cosmos3-Super | ✅ | 3 | 3/3 | 119.03 | **118.51** |
| Wan2.2-I2V-A14B-Diffusers | ✅ | 3 | 3/3 | 201.09 | **201.10** |
| MiniMax-H3 | ✅ | 3 | 3/3 | 77.19 | **77.44** |

## SGLang Server-Side Breakdown

| Model | Server total (s) | Text encode (s) | Denoise (s) | Decode (s) | Median denoise step (ms) |
|-------|------------------|-----------------|--------------|------------|---------------------------|
| Anima-Base-v1.0-Diffusers | 3.25 | 0.02 | 2.99 | 0.22 | 100.55 |
| FLUX.1-dev | 4.29 | 0.04 | 4.08 | 0.02 | 82.00 |
| FLUX.2-dev | 12.90 | 0.36 | 12.08 | 0.01 | 241.77 |
| Qwen-Image-2512 | 8.30 | 0.23 | 8.00 | 0.06 | 160.62 |
| Qwen-Image-Edit-2511 | 14.75 | N/A | 14.02 | 0.10 | 352.43 |
| Z-Image-Turbo | 0.63 | 0.13 | 0.48 | 0.01 | 56.63 |
| Wan2.2-T2V-A14B-Diffusers | 206.30 | 0.27 | 203.47 | 2.24 | 5086.93 |
| Wan2.2-TI2V-5B-Diffusers | 53.08 | 0.34 | 47.94 | 4.75 | 967.48 |
| LTX-2.3 | 12.62 | 0.40 | 8.42 | 1.93 | 278.51 |
| ideogram-4-fp8 | 3.71 | 0.13 | 3.49 | 0.08 | 177.75 |
| Cosmos3-Super | 118.00 | 0.00 | 114.97 | 2.40 | N/A |
| Wan2.2-I2V-A14B-Diffusers | 200.66 | 0.29 | 194.76 | 2.16 | 4865.23 |
| MiniMax-H3 | 76.58 | 0.05 | 73.91 | 1.30 | 1533.35 |

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


## SGLang Performance Trend (Last 30 Runs)

| Date | Commit | anima_base_t2i_1024 (s) | flux1_dev_t2i_1024 (s) | flux2_dev_t2i_1024 (s) | qwen_image_2512_t2i_1024 (s) | qwen_image_edit_2511 (s) | zimage_turbo_t2i_1024 (s) | wan22_t2v_a14b_720p (s) | wan22_ti2v_5b_720p (s) | ltx2.3_twostage_ti2v_2gpus (s) | ideogram4_fp8_t2i_2gpu (s) | cosmos3_super_t2v_2gpu (s) | wan22_i2v_a14b_720p (s) | minimax_h3_t2va_5s (s) | Trend |
|------|--------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|-------|
| Oct 03 | `5b5d721` | 3.26 | 4.47 | 13.02 | 8.37 | 14.83 | 0.76 | 206.80 | 54.51 | 14.73 | 3.81 | 118.51 | 201.10 | 77.44 |             |
|  | `?` | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A | N/A |             |
| Oct 01 | `41cbe65` | 3.31 | 4.46 | 13.12 | 9.02 | 14.92 | 0.77 | 207.96 | 55.06 | 17.30 | 3.83 | 119.24 | 201.70 | 77.45 | :left_right_arrow:  :arrow_up:  :arrow_up:  :arrow_up:  :arrow_up:  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :arrow_up:  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Sep 29 | `98fce73` | 3.25 | 4.28 | 12.38 | 8.16 | 14.43 | 0.64 | 207.65 | 55.19 | 14.05 | 3.71 | 119.42 | 202.62 | 78.24 | :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Sep 29 | `bd78095` | 3.28 | 4.33 | 12.28 | 9.12 | 14.40 | 0.64 | 207.63 | 55.20 | 17.07 | 3.70 | 119.42 | 201.74 | 77.30 | :left_right_arrow:  :arrow_down:  :arrow_down:  :left_right_arrow:  :arrow_down:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Sep 27 | `a0ba196` | 3.31 | 4.45 | 13.12 | 9.24 | 14.92 | 0.78 | 207.66 | 55.15 | 20.08 | 3.82 | 119.34 | 201.67 | 78.20 |  :left_right_arrow:  :left_right_arrow:  :arrow_up:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Sep 25 | `2f5c9ac` | N/A | 4.45 | 13.25 | 8.32 | 14.82 | 0.96 | 207.60 | 56.16 | 13.05 | 3.82 | 118.38 | 201.62 | 77.22 |  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Sep 23 | `172b1b4` | N/A | 4.62 | 13.35 | 8.40 | 14.92 | 0.77 | 207.82 | 56.24 | 14.06 | 3.84 | 119.44 | 201.80 | 78.29 |  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Sep 21 | `50ec970` | N/A | 4.45 | 13.25 | 8.36 | 14.84 | 0.78 | 207.61 | 55.17 | 14.05 | 3.80 | 118.39 | 201.65 | 77.24 |  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Sep 19 | `76f9213` | N/A | 4.47 | 13.37 | 9.04 | 14.93 | 0.76 | 207.69 | 56.18 | 17.07 | 3.82 | 119.38 | 201.66 | 77.24 |  :left_right_arrow:  :left_right_arrow:  :arrow_up:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Sep 17 | `7ccbf5f` | N/A | 4.50 | 13.34 | 8.39 | 14.93 | 0.80 | 206.79 | 56.23 | 13.06 | 3.87 | 119.47 | 201.57 | 78.22 |  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Sep 15 | `832ec39` | N/A | 4.44 | 13.36 | 9.35 | 14.94 | 0.77 | 207.68 | 56.18 | 16.06 | 3.85 | 119.41 | 201.67 | 78.24 |  :left_right_arrow:  :left_right_arrow:  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Sep 13 | `7f1f8c7` | N/A | 4.48 | 13.37 | 8.39 | 14.92 | 0.77 | 207.72 | 56.19 | 13.06 | 3.84 | 119.41 | 202.63 | 78.24 |  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Sep 11 | `ab9750f` | N/A | 4.44 | 13.34 | 10.26 | 15.18 | 0.77 | 207.62 | 56.19 | 29.11 | 3.84 | 119.41 | 201.67 | 78.24 |  :left_right_arrow:  :left_right_arrow:  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Sep 09 | `ffe98a4` | N/A | 4.42 | 13.29 | 8.48 | 15.17 | 0.76 | 206.71 | 55.20 | 14.06 | 3.82 | 118.42 | 201.67 | 77.26 |  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Sep 09 | `0ee8e41` | N/A | 4.43 | 13.34 | 10.03 | 15.18 | 0.80 | 207.69 | 56.20 | 16.07 | 3.83 | 120.38 | 201.67 | 78.25 |  :left_right_arrow:  :left_right_arrow:  :arrow_up:  :left_right_arrow:  :arrow_up:   :left_right_arrow:   :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Sep 07 | `b5c9b68` | N/A | 4.48 | 13.36 | 8.54 | 15.39 | 0.76 | N/A | 56.18 | N/A | 3.83 | 119.39 | 201.68 | 78.25 |  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:   :left_right_arrow:   :left_right_arrow:  :left_right_arrow:   :left_right_arrow: |
| Sep 05 | `dc28438` | N/A | 4.52 | 13.32 | 8.51 | 15.13 | 0.77 | 207.69 | 56.16 | N/A | 3.84 | 119.39 | N/A | 78.22 |  :arrow_down:  :arrow_down:  :arrow_down:  :arrow_down:  :arrow_down:  :left_right_arrow:  :left_right_arrow:   :arrow_down:  :left_right_arrow:   :left_right_arrow: |
| Sep 01 | `00689c0` | N/A | 4.65 | 13.70 | 9.95 | 16.95 | 0.97 | 206.71 | 57.21 | 17.09 | 4.06 | 121.35 | 201.69 | 77.27 |  :left_right_arrow:  :left_right_arrow:  :arrow_up:  :left_right_arrow:  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :arrow_up:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Aug 31 | `52e1c24` | N/A | 4.63 | 13.59 | 8.74 | 16.81 | 0.95 | 207.67 | 57.17 | 14.06 | 4.25 | 120.38 | 201.71 | 77.24 |  :arrow_down:  :left_right_arrow:  :arrow_down:  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Aug 29 | `cdbfe90` | N/A | 5.13 | 13.71 | 10.59 | 16.00 | 0.96 | 206.73 | 57.16 | 17.07 | 4.15 | 120.40 | 202.66 | 77.23 |  :arrow_up:  :left_right_arrow:  :arrow_up:  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Aug 27 | `20a491d` | N/A | 4.58 | 13.49 | 8.90 | 15.26 | 0.95 | 206.73 | 56.17 | 14.06 | 4.12 | 119.41 | 200.67 | 77.26 |  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Aug 25 | `46d9427` | N/A | 4.62 | 13.60 | 8.98 | 15.39 | 0.94 | 207.74 | 56.19 | 14.07 | 4.13 | 120.39 | 201.67 | 77.22 |  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Aug 23 | `de6a1db` | N/A | 4.61 | 13.47 | 8.90 | 15.54 | 0.94 | 206.72 | 56.17 | 13.06 | 4.17 | 119.35 | 200.69 | 77.22 |  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Aug 21 | `a41da99` | N/A | 4.70 | 13.55 | 10.33 | 15.86 | 0.95 | 207.72 | 56.22 | 17.07 | 4.19 | 119.38 | 201.54 | 77.22 |  :arrow_up:  :left_right_arrow:  :arrow_up:  :left_right_arrow:  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :arrow_up:  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Aug 19 | `23f2320` | N/A | 4.44 | 13.38 | 8.84 | 15.68 | 0.78 | 207.75 | 56.19 | 13.05 | 3.98 | 119.37 | 201.65 | 77.21 |  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Aug 19 | `e0ae2e7` | N/A | 4.45 | 13.38 | 10.06 | 15.44 | 0.79 | 207.60 | 56.17 | 17.07 | 4.00 | 119.34 | 201.56 | 77.28 |  :left_right_arrow:  :left_right_arrow:  :arrow_up:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Aug 18 | `0111b29` | N/A | 4.44 | 13.39 | 8.88 | 15.46 | 0.84 | 206.69 | 56.20 | 13.06 | 3.98 | 119.39 | 201.65 | 78.24 |  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :arrow_down:  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow: |
| Aug 18 | `af74337` | N/A | 4.47 | 13.40 | 10.12 | 15.85 | 0.81 | 206.62 | 57.22 | 16.08 | 3.99 | 119.41 | 256.85 | 77.27 |  :arrow_down:  :left_right_arrow:  :arrow_up:  :arrow_up:  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :arrow_up:  :left_right_arrow:  :arrow_up:  :arrow_up:  :left_right_arrow: |
| Aug 15 | `e331baa` | N/A | 4.57 | 13.44 | 8.80 | 15.38 | 0.78 | 206.70 | 56.15 | 13.05 | 4.06 | 115.33 | 201.58 | 77.22 | -- |

> [!CAUTION]
> **Action Required — Performance Alert**
>
> The following cases need attention:
> - zimage_turbo_t2i_1024: SGLang regression +7.3% vs 4-run median (0.76s vs 0.71s)


---
*Generated by `generate_diffusion_dashboard.py` in SGLang nightly CI.*
