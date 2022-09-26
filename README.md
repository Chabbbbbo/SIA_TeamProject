# Detection of Aircraft, Vehicles and Ships in Satellite imagery :: <br/>Team 잘할거SIA
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23#ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Slack](https://img.shields.io/badge/Slack-4A154B?style=for-the-badge&logo=slack&logoColor=white)
![Google Drive](https://img.shields.io/badge/Google%20Drive-4285F4?style=for-the-badge&logo=googledrive&logoColor=white)

<img src = "./img/sia_logo.jpg" style = "width: 100%;">
<br><br>

## 🌈 **팀 구성 및 역할**
<table style = "width:100% !important; margin:0; border:0.5px solid #c1c1c1; font-size:15px;">
    <th style = "width:20%; padding:10px; text-align:center; border:0.5px solid #c1c1c1;">이름</th>
    <th style = "width:20%; padding:10px; text-align:center; border:0.5px solid #c1c1c1;">구성</th>
    <th style = "width:60%; padding:10px; text-align:center; border:0.5px solid #c1c1c1;">역할</th>
    <tr>
        <td style = "padding:10px; text-align:center; border:0.5px solid #c1c1c1;">차보경</td>
        <td style = "padding:10px; text-align:center; border:0.5px solid #c1c1c1;">팀장</td>
        <td style = "padding:10px; text-align:center; border:0.5px solid #c1c1c1;">프로젝트 진행 방향설정, Evaluation Matrix 개선, 모델 학습 및 분석</td>
    </tr>
    <tr>
        <td style = "padding:10px; text-align:center; border:0.5px solid #c1c1c1;">채준병</td>
        <td style = "padding:10px; text-align:center; border:0.5px solid #c1c1c1;">팀원</td>
        <td style = "padding:10px; text-align:center; border:0.5px solid #c1c1c1;">Dataset EDA, 모델 학습 및 분석, large image 처리</td>
    </tr>
    <tr>
        <td style = "padding:10px; text-align:center; border:0.5px solid #c1c1c1;">한연규</td>
        <td style = "padding:10px; text-align:center; border:0.5px solid #c1c1c1;">팀원</td>
        <td style = "padding:10px; text-align:center; border:0.5px solid #c1c1c1;">Dataset EDA, 모델 학습 및 분석</td>
    </tr>
    <tr>
        <td style = "padding:10px; text-align:center; border:0.5px solid #c1c1c1;">임새란</td>
        <td style = "padding:10px; text-align:center; border:0.5px solid #c1c1c1;">팀원</td>
        <td style = "padding:10px; text-align:center; border:0.5px solid #c1c1c1;">라이브러리 구현, 프로젝트 Base line 코드 취합, 모델 학습 및 분석</td>
    </tr>
    <tr>
        <td style = "padding:10px; text-align:center; border:0.5px solid #c1c1c1;">윤혜연</td>
        <td style = "padding:10px; text-align:center; border:0.5px solid #c1c1c1;">팀원</td>
        <td style = "padding:10px; text-align:center; border:0.5px solid #c1c1c1;">모델 결과 시각화 (QGIS 등), 모델 학습 및 분석</td>
    </tr>
</table>
<br/>
<br/>

## 📋 **프로젝트 소개**

### **프로젝트 주제**
위성 영상에서 항공기, 선박, 차량의 위치를 식별한다. 

<ul style = "font-size:15px;">
    <li style = "margin-bottom:20px;"><span style="background-color: #fff5b1">항공기, 선박, 차량 각각 Object Detection</span></li>
    <li style = "margin-bottom:20px;">keyword:  <b>`Object Detection`</b></li>
</ul>
<br/>
<br/>

### 데이터셋 (Fair1M-2.0)
<!-- **Fair1M-2.0** -->
- 데이터셋 정보: [http://gaofenchallenge.com/benchmark](http://gaofenchallenge.com/benchmark)
- 다운로드 링크: [https://drive.google.com/drive/folders/1lCZibAl3k9sI5d7ahRm_5GA3g7OCLXmY?usp=sharing](https://drive.google.com/drive/folders/1lCZibAl3k9sI5d7ahRm_5GA3g7OCLXmY?usp=sharing)
- Gaofan에서 취득한 위성영상
- 600x600 ~ 9472 x 10000 까지 다양한 크기의 Scene 형태
- TIF 확장자로 제공
- GSD(Ground Sample Distance): 0.3m ~ 0.8m
- Label: 객체의 Class, Polygon 등의 정보를 xml 확장자로 제공
<br/>
<br/>

### **프로젝트 레벨 별 스텝**  (순서대로 진행)
<!-- 
---
 -->
- **[LV1] 항공기, 선박, 차량으로만 이루어진 데이터셋으로 정제**
    - 난이도: ★☆☆☆☆ (일반)
    
- **[LV2] 세 가지 Class에 대해 객체 검출을 위한 학습을 수행, 결과 표출**
    - 클래스 별로 각각의 모델을 만들어도 좋습니다.
    - 난이도: ★★☆☆☆ (어려움)

    
- **[LV3] Level2 결과 평가 & 성능 개선**
    - 난이도: ★★★★☆ (어려움)
<br/>
<br/>

## Open Library
<div style = "width:100%; float: left;">
    <div style = "width: 40%; margin-right:10%; float: left;">
      <img src="./img/mmdet-logo.png" width="450"/>
    </div>
    <div style = "width: 40%; margin-right:10%; float: left;">
        <img src = "./img/mmdet-logo.png" width="450"/>
    </div>
</div>
<br/>
<br/>

## ⚒️Baseline Model
### Oriented_RCNN
<img src = "./img/oriented_rcnn.png" style = "width: 100%;">
<br><br>

## EDA 과정
<br><br>

## 문제 해결 및 개선
<br><br>
