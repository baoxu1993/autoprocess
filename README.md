# autoprocess
请在Yii2 2.0.0~2.0.17中使用，其他版本未经测试

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
