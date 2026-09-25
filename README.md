# arc2-code

ARC-AGI-2 (격자 퍼즐) 실험 코드 — arc2 전담 저장소. 계획과 현재 위치는 [`docs/로드맵.md`](docs/로드맵.md).

```
notebooks/
  arc2_desc_lora_v2_colab_h100.ipynb   서술수준 LoRA v2: 27B 교사 채굴 → 왕복 게이트(+무서술 기준선)
                                       → 조립 → QLoRA r64 → 사다리 평가 (셀1~8) — ★정본
```

산출물은 Google Drive `MyDrive/arc_llm/desc_lora/` (노트북이 직접 쓴다).

## arc3-code 와의 관계

- arc3-code 의 브리지(`arc3_lora/requests_to_sft.py`, `sft_encode.py`)가 이 노트북
  **셀7의 행 형식·`encode()` 계약**에 의존한다. 셀7 계약을 바꾸면 arc3 에이전트에게 알린다.
- arc3-code 에 있는 이 노트북 사본은 커밋 `fbe0aeb` 시점 고정본 — 정본은 여기다.
