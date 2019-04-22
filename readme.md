# Opencv
## 第一个例子
### 灰度转换
#### 依赖
`opencv`
`numpy`

```
import cv2
cap = cv2.VideoCapture(0)
gjh = 1
while(True):
    ret,frame = cap.read()
    gray = cv2.cvtColor(frame,cv2.COLOR_BGR2GRAY)
    cv2.imshow('test1',frame)
    cv2.imshow('test2',gray)
    if cv2.waitKey(1) & 0xFF == ord('q'):
        break
cap.release()
cv2.destroyAllWindows()




```