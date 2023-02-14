# Korean_Carplate_Detection / Using Yolov5


Dataset : From AI HUB.



AI HUB의 데이터 100,000장 중에서 약 5,000장 정도를 수작업으로 라벨링 하고, Roboflow에서 제공하는 Data Augmentation 중 Crop을 활용하여 총 12,000장으로 학습 진행.

학습 결과, Confidence는 그렇게 높지 않지만, 그래도 탐지가 되는 경우 나름대로 쓸만한 성능을 보여줌을 알 수 있음.

번호판이 기울어지거나, 화질이 조금 안 좋아지면 탐지 성능이 떨어지는 이슈가 있음.

그런 이슈들은 다른 Repository에 있는 Preprocessing GUI를 사용해, Input Image를 전처리해준 후에 탐지하면 조금 더 나은 결과를 얻을 "수도" 있음.

조금 더 완벽한 결과를 위해서는 ESRGAN이나, HAT-L을 이용해 AI-HUB에서 제공되는 데이터 10만 장을 모두 학습시킨 뒤, 해상도를 높여주는 작업을 하면 좋을 것 같음

Detect.py를 일부 수정해 좀 더 결과를 잘 보이게 하도록 했음.
