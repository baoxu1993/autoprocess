# autoprocess
Eg.
```
    public function afterFind()
    {
        self::setAttributeTransformation('status', 'status_text', self::txtStatus($this->status));//支持方法调用
        self::setAttributeTransformation('create_time', 'create_time_text', date('Y-m-d H:i:s', $this->create_time));//支持直接赋值
    }
```    
Explain.  
>与fields相比更简洁
    ```
    public function fields()
    {
      ........
    }
    ```
