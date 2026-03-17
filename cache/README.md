# cache

This folder is the cache directory for Hugging Face (HF).

When using online mode, downloaded models will be cached in this folder.

For [offline mode](https://huggingface.co/docs/transformers/main/installation#offline-mode) use, please download the models in advance and specify the model directory.


## Directory structures

**There are currently two directory structures:**
- The Huggingface CLI cache structure

### Huggingface CLI cache structure

use this command `tree -a ./cache/huggingface/hub`

```
./cache/huggingface/hub/
├── models--sd2-community--stable-diffusion-2-1-base
│   ├── blobs
│   │   ├── 03d32ad98d2179f954d6754824b3ee8a-10
│   │   ├── 0fa07f924dabbf7517dc62af845cd31573bc09e3
│   │   ├── 28aec93f8557249c72573c9d9c3d489b17fa1254
│   │   ├── 28ec9cf3b239c0751c201b1f6fb46b551df5862731b30a37aa1360101cb3fbab
│   │   ├── 3e4c08995484ee61270175e9e7a072b66a6e4eeb5f0c266667fe1f45b90daf9a
│   │   ├── 469be27c5c010538f845f518c4f5e8574c78f7c8
│   │   ├── 4cafa59ec38fcc84c234a9266d6110bd-10
│   │   ├── 5294955ff7801083f720b34b55d0f1f51313c5c5
│   │   ├── 5df19e76b08f75b3b860de7471ba024b-10
│   │   ├── 65d055d1103982d6ba7cf1c5c876a9413077daf5
│   │   ├── 681c555376658c81dc273f2d737a2aeb23ddb6d1d8e5b3a7064636d359a22668
│   │   ├── 6dfae3e5f7d459b50f4b0850ead945972c75bb0e1897628933e169eb43974214.incomplete
│   │   ├── 76e821f1b6f0a9709293c3b6b51ed90980b3166b
│   │   ├── 7bb11b1da63986aaaaefb5ef2100d34109c024ac640cacd9ed697150c1c57f01
│   │   ├── a434f8fdbb51f080ac57a4377281241467c4efc1417b27646ffae989644de60c
│   │   ├── a722aaa61292631431788c47720ff427-10
│   │   ├── ae0c5be6f35217e51c4c000fd325d8de0294e99c
│   │   ├── b68a817036d3f5c36537e9c332a42c7e63a9d4e9
│   │   ├── c3e254d7b61353497ea0be2c4013df4ea8f739ee88cffa0ba58cd085459ed565
│   │   ├── c7d9f3332a950355d5a77d85000f05e6f45435ea
│   │   ├── c9d67547a136b47c5d4084f6b4f5b222-10
│   │   ├── cce6febb0b6d876ee5eb24af35e27e764eb4f9b1d0b7c026c8c3333d4cfc916c
│   │   ├── d55bbf116323b7e3e80d1f2946f3a2e7-10
│   │   ├── da861650fc7df96390abffcbb9bcf67b7c5566422fda5af9bc003605be65c5f3
│   │   ├── df8958fa5393d70ab11e4c61e56b5d26-10
│   │   ├── df955bdf6b682338ea9b55dfc0d8f3475aadf4836e204893d28b82355e0956d2
│   │   ├── ec130fd46114f8794e55de3feb72ea5b-10
│   │   ├── f537c7f0a35b9b044c51ac5539506b07-10
│   │   ├── f8281be243c1803a2506b38f30f77678-10
│   │   └── f9ac7c0b3b341525cd1b65e1a715128fee97b25c
│   ├── refs
│   │   └── main
│   └── snapshots
│       └── 4e63672c03103b6c636b8fb4119ba982469b2955
│           ├── feature_extractor
│           │   └── preprocessor_config.json -> ../../../blobs/5294955ff7801083f720b34b55d0f1f51313c5c5
│           ├── model_index.json -> ../../blobs/ec130fd46114f8794e55de3feb72ea5b-10
│           ├── README.md -> ../../blobs/28aec93f8557249c72573c9d9c3d489b17fa1254
│           ├── scheduler
│           │   └── scheduler_config.json -> ../../../blobs/b68a817036d3f5c36537e9c332a42c7e63a9d4e9
│           ├── text_encoder
│           │   ├── config.json -> ../../../blobs/f9ac7c0b3b341525cd1b65e1a715128fee97b25c
│           │   ├── model.fp16.safetensors -> ../../../blobs/681c555376658c81dc273f2d737a2aeb23ddb6d1d8e5b3a7064636d359a22668
│           │   ├── model.safetensors -> ../../../blobs/cce6febb0b6d876ee5eb24af35e27e764eb4f9b1d0b7c026c8c3333d4cfc916c
│           │   ├── pytorch_model.bin -> ../../../blobs/c3e254d7b61353497ea0be2c4013df4ea8f739ee88cffa0ba58cd085459ed565
│           │   └── pytorch_model.fp16.bin -> ../../../blobs/7bb11b1da63986aaaaefb5ef2100d34109c024ac640cacd9ed697150c1c57f01
│           ├── tokenizer
│           │   ├── merges.txt -> ../../../blobs/76e821f1b6f0a9709293c3b6b51ed90980b3166b
│           │   ├── special_tokens_map.json -> ../../../blobs/ae0c5be6f35217e51c4c000fd325d8de0294e99c
│           │   ├── tokenizer_config.json -> ../../../blobs/65d055d1103982d6ba7cf1c5c876a9413077daf5
│           │   └── vocab.json -> ../../../blobs/469be27c5c010538f845f518c4f5e8574c78f7c8
│           ├── unet
│           │   ├── config.json -> ../../../blobs/0fa07f924dabbf7517dc62af845cd31573bc09e3
│           │   ├── diffusion_pytorch_model.bin -> ../../../blobs/a434f8fdbb51f080ac57a4377281241467c4efc1417b27646ffae989644de60c
│           │   ├── diffusion_pytorch_model.fp16.bin -> ../../../blobs/da861650fc7df96390abffcbb9bcf67b7c5566422fda5af9bc003605be65c5f3
│           │   ├── diffusion_pytorch_model.fp16.safetensors -> ../../../blobs/28ec9cf3b239c0751c201b1f6fb46b551df5862731b30a37aa1360101cb3fbab
│           │   └── diffusion_pytorch_model.safetensors -> ../../../blobs/4cafa59ec38fcc84c234a9266d6110bd-10
│           ├── v2-1_512-ema-pruned.ckpt -> ../../blobs/c9d67547a136b47c5d4084f6b4f5b222-10
│           ├── v2-1_512-ema-pruned.safetensors -> ../../blobs/df955bdf6b682338ea9b55dfc0d8f3475aadf4836e204893d28b82355e0956d2
│           ├── v2-1_512-nonema-pruned.ckpt -> ../../blobs/df8958fa5393d70ab11e4c61e56b5d26-10
│           ├── v2-1_512-nonema-pruned.safetensors -> ../../blobs/03d32ad98d2179f954d6754824b3ee8a-10
│           └── vae
│               ├── config.json -> ../../../blobs/f537c7f0a35b9b044c51ac5539506b07-10
│               ├── diffusion_pytorch_model.bin -> ../../../blobs/5df19e76b08f75b3b860de7471ba024b-10
│               ├── diffusion_pytorch_model.fp16.bin -> ../../../blobs/a722aaa61292631431788c47720ff427-10
│               ├── diffusion_pytorch_model.fp16.safetensors -> ../../../blobs/3e4c08995484ee61270175e9e7a072b66a6e4eeb5f0c266667fe1f45b90daf9a
│               └── diffusion_pytorch_model.safetensors -> ../../../blobs/d55bbf116323b7e3e80d1f2946f3a2e7-10
├── version_diffusers_cache.txt
└── version.txt

12 directories, 60 files
```

## Pre-download for offline mode

Running in online mode will automatically download the model.

### use huggingface-cli

install cli

```bash
pip install -U "huggingface_hub[cli]"
```

download model

```bash
hf download sd2-community/stable-diffusion-2-1-base --cache-dir ./cache/huggingface/hub
hf download sd2-community/stable-diffusion-2-1 --cache-dir ./cache/huggingface/hub
hf download stabilityai/stable-diffusion-xl-base-1.0 --cache-dir ./cache/huggingface/hub
hf download CompVis/stable-diffusion-v1-4 --cache-dir ./cache/huggingface/hub
hf download stable-diffusion-v1-5/stable-diffusion-v1-5 --cache-dir ./cache/huggingface/hub
```
