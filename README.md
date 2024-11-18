```
[2024-11-18 21:51:28,038 submission_checker1.py:3109 INFO] Results=3, NoResults=0, Power Results=0
[2024-11-18 21:51:28,038 submission_checker1.py:3116 INFO] ---
[2024-11-18 21:51:28,038 submission_checker1.py:3117 INFO] Closed Results=0, Closed Power Results=0

[2024-11-18 21:51:28,038 submission_checker1.py:3122 INFO] Open Results=3, Open Power Results=0

[2024-11-18 21:51:28,038 submission_checker1.py:3127 INFO] Network Results=0, Network Power Results=0

[2024-11-18 21:51:28,038 submission_checker1.py:3132 INFO] ---
[2024-11-18 21:51:28,038 submission_checker1.py:3134 INFO] Systems=3, Power Systems=0
[2024-11-18 21:51:28,038 submission_checker1.py:3138 INFO] Closed Systems=0, Closed Power Systems=0
[2024-11-18 21:51:28,038 submission_checker1.py:3143 INFO] Open Systems=3, Open Power Systems=0
[2024-11-18 21:51:28,038 submission_checker1.py:3148 INFO] Network Systems=0, Network Power Systems=0
[2024-11-18 21:51:28,038 submission_checker1.py:3153 INFO] ---
[2024-11-18 21:51:28,038 submission_checker1.py:3158 INFO] SUMMARY: submission looks OK
INFO:root:       ! call "postprocess" from /home/runner/CM/repos/mlcommons@cm4mlops/script/run-mlperf-inference-submission-checker/customize.py

```

|    | Organization   | Availability   | Division   | SystemType   | SystemName   | Platform                                                      | Model               | MlperfModel         | Scenario   |   Result | Accuracy                                                     |   number_of_nodes | host_processor_model_name        |   host_processors_per_node |   host_processor_core_count | accelerator_model_name   |   accelerators_per_node | Location                                                                                                    | framework      | operating_system                                | notes                             |   compliance |   errors | version   |   inferred | has_power   | Units     | weight_data_types   |
|---:|:---------------|:---------------|:-----------|:-------------|:-------------|:--------------------------------------------------------------|:--------------------|:--------------------|:-----------|---------:|:-------------------------------------------------------------|------------------:|:---------------------------------|---------------------------:|----------------------------:|:-------------------------|------------------------:|:------------------------------------------------------------------------------------------------------------|:---------------|:------------------------------------------------|:----------------------------------|-------------:|---------:|:----------|-----------:|:------------|:----------|:--------------------|
|  0 | NTHU           | available      | open       | datacenter   | 334907abd4f4 | Kuai-Kuai_702-reference-gpu-pytorch-v2.5.1-scc24-base_cu124   | stable-diffusion-xl | stable-diffusion-xl | Offline    | 0.528528 | CLIP_SCORE: 16.4035627245903  FID_SCORE: 235.76925470141796  |                 1 | INTEL(R) XEON(R) PLATINUM 8592+  |                          2 |                          64 | NVIDIA H100 PCIe         |                       4 | open/NTHU/results/Kuai-Kuai_702-reference-gpu-pytorch-v2.5.1-scc24-base_cu124/stable-diffusion-xl/offline   | pytorch v2.5.1 | Ubuntu 22.04 (linux-6.8.0-47-generic-glibc2.35) | Automated by MLCommons CM v3.1.0. |            1 |        0 | v4.1      |          0 | False       | Samples/s | fp32                |
|  1 | NTHU           | available      | open       | datacenter   | ba7f5c94d10f | ba7f5c94d10f-nvidia-gpu-TensorRT-scc24-base                   | stable-diffusion-xl | stable-diffusion-xl | Offline    | 4.2742   | CLIP_SCORE: 31.234263841211796  FID_SCORE: 23.67815832489498 |                 1 | INTEL(R) XEON(R) PLATINUM 8592+  |                          2 |                          64 | NVIDIA H100 PCIe         |                       4 | open/NTHU/results/ba7f5c94d10f-nvidia-gpu-TensorRT-scc24-base/stable-diffusion-xl/offline                   | TensorRT       | Ubuntu 22.04 (linux-6.8.0-47-generic-glibc2.35) | Automated by MLCommons CM v3.4.1. |            1 |        0 | v4.1      |          0 | False       | Samples/s | int8                |
|  2 | scc2           | available      | open       | datacenter   | f2ea47b0a016 | f2ea47b0a016-nvidia_original-gpu-tensorrt-vdefault-scc24-main | stable-diffusion-xl | stable-diffusion-xl | Offline    | 7.46497  | CLIP_SCORE: 16.63159880042076  FID_SCORE: 234.62921308614995 |                 1 | AMD EPYC 9754 128-Core Processor |                          2 |                         128 | NVIDIA H100 80GB HBM3    |                       6 | open/scc2/results/f2ea47b0a016-nvidia_original-gpu-tensorrt-vdefault-scc24-main/stable-diffusion-xl/offline | TensorRT       | Ubuntu 20.04 (linux-6.1.0-27-amd64-glibc2.31)   | Automated by MLCommons CM v3.3.3. |            1 |        0 | v4.1      |          0 | False       | Samples/s | int8                |