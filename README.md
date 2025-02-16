deepseek等系列蒸馏模型本地部署测试，欢迎补充
| gpu      | cpu     | model                  | token/s | sm%   | mem%  | pcie/Ms | pwr/W | server  |
|----------|---------|------------------------|---------|-------|-------|---------|-------|---------|
| 3090x4   | 4309y   | unsloth/70b/Q4_K_M     | 16.77   | 14-30 | 14-30 | 65      |       | ollama  |
| 3090x2   | 4309y   | unsloth/70b/Q4_K_M     | 17.07   | 42-56 | 40-60 | 90      |       | ollama  |
| 3090x4   | 4309y   | deepseek/32b/BF16      | 33.7    | 85-94 | 73-78 | 820     |       | vllm    |
| P40x1    | 2680v4  | unsloth/32b/Q4_K_M     | 6.46    | 96-98 | 80-82 | ?       | 211   | ollama  |
| 4090x2   | 13900K  | unsloth/70b/Q4 KM      | 19.49   | 48-50 | 51-54 | 78      | 223   | ollama  |
| 4090x4   | 13900K  | unsloth/70b/Q4_K_M     | 19.49   | 22-26 | 22-28 | 58      | 128   | ollama  |
| 2080tix2 | 7920X   | unsloth/70b/Q4_K_M     | 8.8     | 36-38 | 36-40 | 65      | 193   | ollama  |
| 2080tix1 | 7920X   | unsloth/32b/Q4_K_M     | 21.94   | 94-95 | 87-89 | 89      | 258   | ollama  |
| M40x1    | 7920X   | unsloth/32b/Q4_K_M     | 6.45    | 96-98 | 67-68 | 35      | 232   | ollama  |
| v100x4   | 4210    | unsloth/70b/Q4_K_M     | 13.87   | 19-22 | 19-28 | ?       | 171   | ollama  |
| v100x2   | 4210    | unsloth/70b/Q4_K_M     | 14.08   | 38-56 | 37-52 | ?       | 250   | ollama  |
| v100x1   | 4210    | unsloth/32b/Q4_K_M     | 25.47   | 86-87 | 76-77 | ?       | 221   | ollama  |
| 4060ti   | 2680v4x2| llama3:70b             | 4.3     |       |       |         |       |         |
|RadeonVIIx4|        |deepseek-r1-distill-llama-70b|7.64|       |       |         |       |LM-Studio|
| 2080ti22g| 2673v3  | deepseek-r1:32b        | 20.79   |       |       |         |       | ollama  |
| 2080ti11g| 13700kf | deepseek-r1:14b        | 11      |       |       |         |       |         |
| v100x2   | XEON3 ESx2 | deepseek-r1:671b/Q4      | 6.4   |       |       |         |       | ollama |

感谢八云紫提供的测试数据
