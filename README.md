# EasyCameraExt

根据 https://github.com/Glamdring/EasyCamera 改写。

使用：
 
 (1) 启动：
 
 `startActivityForResult( new Intent(ChatActivity.this, EasyCameraActivity.class), REQUEST_CODE_CAMERA);`

 (2) 获取拍照结果(目前仅返回照片在sd卡上的目录)：
```
protected void onActivityResult(int requestCode, int resultCode, Intent data) {
		super.onActivityResult(requestCode, resultCode, data);
		if(data.hasExtra(EasyCameraActivity.RESULE_IMAGE_PATH)){
			String imagePaht = data.getStringExtra(EasyCameraActivity.RESULE_IMAGE_PATH);
		}
}
```
(3) 界面效果:

![界面效果(http://img.blog.csdn.net/20150729150309253)
