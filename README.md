# llama-70b-chat-4-shards

This repository contains a script to transform the weights of Llama v2 70B (chat) from an 8-shard configuration to a 4-shard configuration, making it more accessible for users with machines that have only 4 GPUs.

## Introduction

Meta recently released the weights for Llama v2 70B, distributed across 8 shards. However, some users may have hardware constraints, such as having only 4 GPUs on their machine, making it difficult to load and utilize the model directly. This repository provides a solution to this problem by offering a script that can transform the 8-shard weight distribution of LLAMA v2 70B into a 4-shard configuration, facilitating easier usage on machines with fewer GPUs.

## Usage

```
python convert.py \
    --input_llama_path ~/llama-2-70b-chat \
    --input_shards 8 \
    --output_llama_path ~/llama-2-70b-chat-4-shards \
    --output_shards 4
```

## Acknowledgements

- Thanks to Meta for releasing the Llama v2 70B weights.
- Any other acknowledgements or credits you'd like to give.

## Contact

For any inquiries or to report issues, please open an issue on this repository or contact the repository owner at your@email.com.
