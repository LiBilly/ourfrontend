# CSS Position(定位) & Float(浮动)

## Position
> 1. 包含4个值:static,relative,absolute,fixed,默认值:static
> 2. 可用于所有元素
> 3. 不能继承

### **static**
元素的位置遵循默认标准文档流

### **relative**
元素的位置将偏移它在认标准文档流中的位置

### **absolute**
脱离标准文档流,根据属性形成在相对应元素(拥有position:relative|absolute|fixed)父类或祖先类元素)里的独立位置

### **fixed**
脱离标准文档流,固定以页面某个位置


## Float
> 1. 包含3个值:left,right,none,默认值none
> 2. 可用于所有元素
> 3. 不能继承