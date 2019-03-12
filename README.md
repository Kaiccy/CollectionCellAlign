# CollectionCellAlign
使得collectionCell 居中，靠左或者靠右。

项目中发现当collectionView只有一个cell 的时候，默认cell是居中的。但是我们产品可能是要求靠左的，这是时就需要自定义一个继承自UICollectionViewFlowLayout 的类，来设置cell 的布局。重写 layoutAttributesForElementsInRect 方法。

使用：

将CollectionViewcellAlignLayout.h 和 CollectionViewcellAlignLayout.m 文件拖入自己的工程中。

//betweenOfCell 为每个cell 之间的距离。

CollectionViewcellAlignLayout *layout = [[CollectionViewcellAlignLayout alloc]initWithType:AlignWithLeft betweenOfCell:10.0];

[_collectionV setCollectionViewLayout:layout];
