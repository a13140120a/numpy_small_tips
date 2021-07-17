# numpy_small_tips


* 間隔切片
    ```py
    a = np.arange(10)
    # [0 1 2 3 4 5 6 7 8 9]
    s = slice(2,7,2)   #從索引 2 到索引 7 停止，間隔為2
    print (a[s])
    # output: [2  4  6]
    ```
* 限定範圍:
    ```py
    # 所有值必須介於 0~255 之間，超過255 = 255，小於 0 = 0
    img = np.clip(img, 0, 255)
    ```
