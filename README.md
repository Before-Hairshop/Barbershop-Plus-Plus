# AI Beforehairshop

## Prerequisite
- Barbershop/unprocessed 폴더와 Barbershop/input/face 폴더 생성
- 변경시킬 수 있는 헤어스타일 이미지는 미리 W+ space 상에서 encoding 된 latent vector가 있어야 한다.


## Download II2S images
Please download the [II2S](https://drive.google.com/drive/folders/15jsR9yy_pfDHiS9aE3HcYDgwtBbAneId?usp=sharing) 
and put them in the `Barbershop/input/face` folder.

## Inference

`./Barbershop-inference.ipynb` 파일을 확인해주시기 바랍니다. 

pSp 인코딩 후, Barbershop/output/W+ 폴더에 .npy 파일 저장

```shell
# unprocessed 폴더에 있는 파일의 얼굴을 alignment하고, 자동으로 input/face 폴더에 이미지 생성
!python align_face.py
```

```shell
# 예시 script
!python main.py --im_path1 input_img2.png --im_path2 117.png --im_path3 117.png --sign realistic --smooth 1
```

