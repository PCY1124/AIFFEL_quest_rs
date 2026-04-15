# AIFFEL Campus Online Code Peer Review Templete
- 코더 : 박찬영
- 리뷰어 : 정주열


# PRT(Peer Review Template)
- [x]  **1. 주어진 문제를 해결하는 완성된 코드가 제출되었나요?**
    - 문제에서 요구하는 최종 결과물이 첨부되었는지 확인
        - 아래와 같이 train loss와 validation loss가 수렴하는것을 볼 수 있고, early stopping을 해서 오버피팅을 방지했습니다.
        - 또한 seq2seq와 어텐션을 이용해서 핵심 정보는 일부 잡는 결과를 보여줬습니다.
    <img width="559" height="409" alt="image" src="https://github.com/user-attachments/assets/c492f202-83ca-415f-a57b-565a550fa5ba" />
    <img width="1421" height="720" alt="image" src="https://github.com/user-attachments/assets/64ea5bec-bed1-4395-b378-e8f4ab015ca1" />

- [x]  **2. 전체 코드에서 가장 핵심적이거나 가장 복잡하고 이해하기 어려운 부분에 작성된 
주석 또는 doc string을 보고 해당 코드가 잘 이해되었나요?**
    - 해당 코드 블럭을 왜 핵심적이라고 생각하는지 확인
    - 해당 코드 블럭에 doc string/annotation이 달려 있는지 확인
    - 해당 코드의 기능, 존재 이유, 작동 원리 등을 기술했는지 확인
    - 주석을 보고 코드 이해가 잘 되었는지 확인
        - 학습이 끝난 이후에 추론모델이 학습 모델과 디코더를 달리 해야하는데 주석을 블럭마다 작성되어서 이해하기 쉬웠습니다.
        - 그리고 "학습된 Seq2Seq 모델을 사용하여 새로운 요약문을 생성하기 위한 추론 모델을 설계합니다. 인코더와 디코더를 분리하여 예측 과정에 맞게 재구성합니다."라는 멘트가 있어서 좋았습니다.
    <img width="882" height="534" alt="image" src="https://github.com/user-attachments/assets/031bc8a7-04fd-4b8b-9cc8-950faf813d8a" />

        
- [ ]  **3. 에러가 난 부분을 디버깅하여 문제를 해결한 기록을 남겼거나
새로운 시도 또는 추가 실험을 수행해봤나요?**
    - 문제 원인 및 해결 과정을 잘 기록하였는지 확인
    - 프로젝트 평가 기준에 더해 추가적으로 수행한 나만의 시도, 
    실험이 기록되어 있는지 확인
        - 추상적 요약 부분에서 결과 해석이 아래와 같이 되어 있는데 결과 분석 부분에서는 좋았습니다. 하지만 새로운 시도나 추가 실험은 없어서 아쉬웠습니다.
    <img width="497" height="155" alt="image" src="https://github.com/user-attachments/assets/2e4781df-12d7-4264-b04e-e65d56e63bf2" />

- [x]  **4. 회고를 잘 작성했나요?**
    - 주어진 문제를 해결하는 완성된 코드 내지 프로젝트 결과물에 대해
    배운점과 아쉬운점, 느낀점 등이 기록되어 있는지 확인
    - 전체 코드 실행 플로우를 그래프로 그려서 이해를 돕고 있는지 확인
        - 아래와 같이 추상적 요약과 추출적 요약 결과 비교 및 분석을 표를 통해 잘 제시했고, 분석결과(회고)를 잘 작성했습니다. 각 요약의 장점과 단점을 비교분석했고, 어디서 성능개선이 필요한지 언급되어 있습니다. 
    <img width="1399" height="551" alt="image" src="https://github.com/user-attachments/assets/c5169be0-e5fb-47ab-9076-88aa2e6fbfd6" />

        
- [x]  **5. 코드가 간결하고 효율적인가요?**
    - 파이썬 스타일 가이드 (PEP8) 를 준수하였는지 확인
    - 코드 중복을 최소화하고 범용적으로 사용할 수 있도록 함수화/모듈화했는지 확인
        - 데이터 전처리 부분에서 텍스트 정규화를 위한 함수 정의, 불용어 제거 부분을 함수화해서 깔끔하게 사용되었습니다.
    <img width="752" height="424" alt="image" src="https://github.com/user-attachments/assets/c121b258-6b3b-451c-b7cd-8daa3c6c4e06" />


# 회고(참고 링크 및 코드 개선)
데이터 전처리 -> 모델 설계 -> 모델 학습 -> 테스트 -> 결과 비교 까지 전체적인 흐름이 깔끔해서 한눈에 들어와서 읽기 좋았습니다. 또한 마지막에 분석 결과 내용을 읽으며 위에 나온 추상적 요약과 추출적 요약 결과를 동시에 봤는데 정말 잘 분석된 것 같습니다. 공감을 하며 읽었습니다. 

