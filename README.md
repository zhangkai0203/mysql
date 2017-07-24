# mysql

#### mysql中的username='%s' and xx='%f'"表示什么意思？

    $Model->where("id=%d and username='%s' and xx='%f'",array($id,$username,$xx))->select();
    // 或者
    $Model->where("id=%d and username='%s' and xx='%f'",$id,$username,$xx)->select();
   
    类似于于sprintf("id=%d and %s", $val, $str);是格式化的意思，%s代表字符串，%f表示浮点数！
