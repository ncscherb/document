
## 缓存添加的商品信息
- 在后台添加商品信息时生成对应商品的详细信息静态页面
- 在前台访问该商品时，直接访问该商品的后台生成的静态页面
#### 注意问题：
- 后台访问前台视图模板的方法：$this->(Home@Goods/index)

```
    ob_start();

    $this->assign("info",$_POST);
	//调用前台View/Good中的detail.html
    $this->display("Home@Goods/detail");

    $content=ob_get_contents();

    file_put_contents("./Public/CachedHtml/Goods/goods_".$row.".html",$content);
    ob_end_clean();

    $this->redirect("Admin/Goods/showlist",array(),2,"添加成功");
```