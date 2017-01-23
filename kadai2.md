2階調，4階調，8階調での画像の表示を行い，それによる移り変わり，及び階調特性による擬似輪郭を確認する．  

ORG=imread(0.jpg); % 原画像の入力  

原画像を読み込み，表示した結果を図１に示す．

![原画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/0.jpg?raw=true)  
図1 原画像
結果を図2に示す．

![原画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/0-1.jpg?raw=true)  
図2 2階調画像

2階調画像の生成は次のように行う．

IMG = ORG>128;
imagesc(IMG); colormap(gray); colorbar;  axis image;

結果を図3に示す．

![原画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/0-2.jpg?raw=true)  
図3 4階調画像


4階調画像の生成は次のように行う．

![原画像](https://github.com/ariga11029/lecture_image_processing/blob/master/image/0-3.jpg?raw=true)  
図4 8階調画像
