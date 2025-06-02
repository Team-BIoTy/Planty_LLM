<img alt="Python" src="https://img.shields.io/badge/Python-3776AB.svg?style=for-the-badge&logo=Python&logoColor=white" height="20"/> <img alt="HuggingFace" src="https://img.shields.io/badge/HuggingFace-FFD21E.svg?style=for-the-badge&logo=HuggingFace&logoColor=white" height="20"/>


# 🌱 Planty_LLM

**Planty Agent**에서 사용한 BaseModel 파인튜닝 코드입니다.

### 프로젝트 개요
- **기간**: 2025.03.12 - 2025.05.14
- **목표**: 파인튜닝을 통해 로컬 환경에서 동작할 수 있는 식물 SLM 개발발 
- 파인튜닝을 완료한 모델은 [Planty Agent](https://github.com/Team-BIoTy/Planty_Agent)에서 에이전트 구현에 사용하였습니다. 

</br>

 ## 🤖 모델 소개

| **모델** | **식물 정보 정확성** | **평균 답변 적절성** | **모델 사이즈(MB)** | **응답시간 (s)** | ox 정답률 |
| --- | --- | --- | --- | --- | --- |
| **gemma-3-4b (기본 모델)** | 8.59 | 8.76 | 16403.70 | 36.25 | 84 |
| **gemma_sft** | 8.88 | 8.58 | 12.33 | 42.07 | 84 |
| **gemma-3-4b-planty-2** | 7.5 | 7.24 | 45.46 | 47.16 | 88 |
| **gemma-3-4b-planty-ia3** | 9.12 | 8.53 | 1.65 | 41.26 | 82 |
| **HyperCLOVAX-SEED-Text-Instruct-1.5B (기본 모델)** | 6.6 | 6.2 | 6048 | 7.07 | 54 |
| **HyperCLOVAX-SEED-Text-Instruct-1.5B-planty-ia3** | 6.31 | 6.17 | 0.76 | 8.80 | 54 |
| **HyperCLOVAX-SEED-Text-Instruct-1.5B-planty-ia3-2** | 6.58 | 6.35 | 0.76 | 10.06 | 54 |

- **[gemma-3-4b](https://huggingface.co/google/gemma-3-4b-it)**: google에서 개발한 gemma-3-4b-it, base model
- **[gemma_sft](https://huggingface.co/yerim00/gemma_sft)**: base model + QLoRA
- **[gemma-3-4b-it-planty-2](https://huggingface.co/yerim00/gemma-3-4b-it-planty-2)**: base model + QLoRA (파라미터 변경)
- **[gemma-3-4b-planty-ia3](https://huggingface.co/yerim00/gemma-3-4b-it-planty-ia3)**: base model + IA3
- **[HyperCLOVAX-SEED-Text-Instruct-1.5B](https://huggingface.co/naver-hyperclovax/HyperCLOVAX-SEED-Text-Instruct-1.5B)**: naver에서 개발한 HyperCLOVAX-SEED-Text-Instruct-1.5B, base model
- **[HyperCLOVAX-SEED-Text-Instruct-1.5B-planty-ia3](https://huggingface.co/yerim00/HyperCLOVAX-SEED-Text-Instruct-1.5B-planty-ia3)**: base model + IA3
- **[HyperCLOVAX-SEED-Text-Instruct-1.5B-planty-ia3-2](https://huggingface.co/yerim00/HyperCLOVAX-SEED-Text-Instruct-1.5B-planty-ia3-2)**: base model + IA3 (파라미터 변경)
