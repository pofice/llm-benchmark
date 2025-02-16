# llm-benchmark
deepseek系列蒸馏模型本地部署测试
| id | cpu    | gpu      | model                  | token/s | sm%   | mem%  | pcie/Ms | pwr/W | server  |
|----|--------|----------|------------------------|---------|-------|-------|---------|-------|---------|
| 0  | 4309y  | 3090x4   | unsloth/70b/Q4_K_M     | 16.77   | 14-30 | 14-30 | 65      |       | ollama  |
| 1  | 4309y  | 3090x2   | unsloth/70b/Q4_K_M     | 17.07   | 42-56 | 40-60 | 90      |       | ollama  |
| 2  | 4309y  | 3090x4   | deepseek/32b/BF16      | 33.7    | 85-94 | 73-78 | 820     |       | vllm    |
| 3  | 2680v4 | P40x1    | unsloth/32b/Q4_K_M     | 6.46    | 96-98 | 80-82 | ?       | 78    | 211     |
| 4  | 13900K | 4090x2   | unsloth/70b/Q4 KM      | 19.49   | 48-50 | 51-54 | 78      | 223   | ollama  |
| 5  | 13900K | 4090x4   | unsloth/70b/Q4_K_M     | 19.49   | 22-26 | 22-28 | 58      | 128   | ollama  |
| 6  | 7920X  | 2080tix2 | unsloth/70b/Q4_K_M     | 8.8     | 36-38 | 36-40 | 65      | 193   | ollama  |
| 7  | 7920X  | 2080tix1 | unsloth/32b/Q4_K_M     | 21.94   | 94-95 | 87-89 | 89      | 258   | ollama  |
| 8  | 7920X  | M40x1    | unsloth/32b/Q4_K_M     | 6.45    | 96-98 | 67-68 | 35      | 232   | ollama  |
| 9  | 4210   | v100x4   | unsloth/70b/Q4_K_M     | 13.87   | 19-22 | 19-28 | ?       | 171   | ollama  |
| 10 | 4210   | v100x2   | unsloth/70b/Q4_K_M     | 14.08   | 38-56 | 37-52 | ?       | 250   | ollama  |
| 11 | 4210   | v100x1   | unsloth/32b/Q4_K_M     | 25.47   | 86-87 | 76-77 | ?       | 221   | ollama  |
