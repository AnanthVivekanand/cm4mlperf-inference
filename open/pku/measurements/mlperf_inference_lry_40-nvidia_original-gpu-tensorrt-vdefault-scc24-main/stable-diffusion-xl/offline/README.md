This experiment is generated using the [MLCommons Collective Mind automation framework (CM)](https://github.com/mlcommons/cm4mlops).

*Check [CM MLPerf docs](https://docs.mlcommons.org/inference) for more details.*

## Host platform

* OS version: Linux-5.14.0-427.33.1.el9_4.x86_64-x86_64-with-glibc2.29
* CPU version: x86_64
* Python version: 3.8.10 (default, Sep 11 2024, 16:02:53) 
[GCC 9.4.0]
* MLCommons CM version: 3.4.1

## CM Run Command

See [CM installation guide](https://docs.mlcommons.org/inference/install/).

```bash
pip install -U cmind

cm rm cache -f

cm pull repo mlcommons@cm4mlops --checkout=852b297c18a90edb8a9c975dd7ee7cf731e1e347

cm run script \
	--tags=run-mlperf,inference,_r4.1-dev,_scc24-main \
	--model=sdxl \
	--implementation=nvidia \
	--max_query_count=5000 \
	--min_query_count=72 \
	--framework=tensorrt \
	--category=datacenter \
	--scenario=Offline \
	--execution_mode=test \
	--device=cuda \
	--max_batchsize=8 \
	--quiet \
	--rerun
```
*Note that if you want to use the [latest automation recipes](https://docs.mlcommons.org/inference) for MLPerf (CM scripts),
 you should simply reload mlcommons@cm4mlops without checkout and clean CM cache as follows:*

```bash
cm rm repo mlcommons@cm4mlops
cm pull repo mlcommons@cm4mlops
cm rm cache -f

```

## Results

Platform: mlperf_inference_lry_40-nvidia_original-gpu-tensorrt-vdefault-scc24-main

Model Precision: int8

### Accuracy Results 
`CLIP_SCORE`: `14.02827`, Required accuracy for closed division `>= 31.68632` and `<= 31.81332`
`FID_SCORE`: `84.33062`, Required accuracy for closed division `>= 23.01086` and `<= 23.95008`

### Performance Results 
`Samples per second`: `8.00134`
