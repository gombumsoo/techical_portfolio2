# techical_portfolio2

## 기술 평가 항목
1. Python, SQL, R, Java, Scala, Go, C/C++, Javascript 등 데이터 처리 언어 활용 능력
---
## 레포지토리 소개
본 레포지토리는 KAMP에서 제공하는 [에너지(전력) 사용량 데이터](https://www.kamp-ai.kr/aidataDetail?AI_SEARCH=%EC%A0%84%EA%B8%B0&page=1&DATASET_SEQ=27&EQUIP_SEL=&GUBUN_SEL=&FILE_TYPE_SEL=&WDATE_SEL=)에 있는 여러 변수를 활용해 일일 평균 전기 사용량을 예측하는 LSTM모델을 학습하고, 결과를 정리한 것입니다. Modeling_LSTM.ipynb파일에서 진행했습니다.

### 진행 과정
- pandas 라이브러리를 통해 csv 형태의 데이터를 DataFrame형태로 불러오고, 이후 모델의 학습에 적절하게 sklearn라이브러리를 사용해 강수량 변수에 대한 binarization을 진행했습니다.
![image](https://github.com/gombumsoo/techical_portfolio2/assets/69720752/37f9e8fb-6c68-4f2a-a794-1a0ed6b91a26)
![image](https://github.com/gombumsoo/techical_portfolio2/assets/69720752/214eb306-53ed-4ba3-b43c-4dd21aa8a5ae)
- 이후 일일 전기 사용량 예측 모델 학습/평가를 위해 tensorflow를 활용했고, training loss function과 test data에 대한 예측 결과를 나타내기 위해 matplotlib 라이브러리를 사용했습니다.
- 적적한 hyperparameter를 설정하여 학습한 결과, train/validation loss가 수렴한 것을 확인했고, 이후 test set에 대한 prediction과 ground truth를 비교해본 결과 일부 기간을 제외하고 어느정도 유사한 값을 예측하는 것을 확인했습니다.
![image](https://github.com/gombumsoo/techical_portfolio2/assets/69720752/a048a850-5f9a-42aa-a53d-807f99600ddc)
![image](https://github.com/gombumsoo/techical_portfolio2/assets/69720752/f5ae185c-61d7-4f55-a7b0-d9cd919dff02)



