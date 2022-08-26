# Detection of Aircraft, Vehicles and Ships in Satellite imagery :: Team 잘할거SIA

## 📋 **프로젝트 소개**

### **프로젝트 주제**

---

위성 영상에서 항공기, 선박, 차량의 위치를 식별한다. 

- 항공기, 선박, 차량 각각 Object Detection
- keyword:  **`Object Detection`**

### 데이터셋

---

**Fair1M-2.0**

- 데이터셋 정보: [http://gaofenchallenge.com/benchmark](http://gaofenchallenge.com/benchmark)
- 다운로드 링크: [https://drive.google.com/drive/folders/1lCZibAl3k9sI5d7ahRm_5GA3g7OCLXmY?usp=sharing](https://drive.google.com/drive/folders/1lCZibAl3k9sI5d7ahRm_5GA3g7OCLXmY?usp=sharing)
- Gaofan에서 취득한 위성영상
- 600x600 ~ 9472 x 10000 까지 다양한 크기의 Scene 형태
- TIF 확장자로 제공
- GSD(Ground Sample Distance): 0.3m ~ 0.8m
- Label: 객체의 Class, Polygon 등의 정보를 xml 확장자로 제공

### **프로젝트 레벨 별 스텝**  (순서대로 진행)

---

- **[LV1] 항공기, 선박, 차량으로만 이루어진 데이터셋으로 정제**
    - 난이도: ★☆☆☆☆ (일반)
    
- **[LV2] 세 가지 Class에 대해 객체 검출을 위한 학습을 수행, 결과 표출**
    - 클래스 별로 각각의 모델을 만들어도 좋습니다.
    - 난이도: ★★☆☆☆ (어려움)

    
- **[LV3] Level2 결과 평가 & 성능 개선**
    - 난이도: ★★★★☆ (어려움)
        
