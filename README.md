# Project: UF Event Marking_yoloV5

Event Marking 구현을 위한 yolov5 알고리즘 구현입니다.

 Project : Uniformity Event Marking

#1. Summary

 - 알고리즘 : YOLO V5
 - labeling tool : labelimg / https://github.com/tzutalin/labelImg.git
 - label : Tire Outter / Tire Inner / Barcode
 
#2. Labeling tool 사용법
 1) git clone https://github.com/tzutalin/labelImg.git
 2) 설치폴더의 /data/predefined_class.txt 수정
    본 Project의 경우 Tire 외경/내경/Barcode 검출이 필요함으로 Tire / Tire_inner / Barcode로 정의
    추후 Marking, 등급에 대한 구분도 try 필요
 3) cmd 창의 해당 폴더에서, python labelimg.py 실행
  - Open Dir에서 사진이 있는 폴더 선택
  - Change Save Dir에서 Labeling 결과물이 나오는 폴더 선택
  - Save 밑에 YOLO 선택, ('PascalVOC', 'CreateML', 'Yolo' 세가지 옵션으로 되어있음)
  - Labeling 작업 진행
  
#3. Yolo V5 사용법
 - Training_YOLOV5.ipynb 파일 참조
 - best.pt파일을 활용하여 detect.py파일 활용하여 사용
