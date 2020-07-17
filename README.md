# iconv_test
iconv의 인코딩을 여러가지 확인할 수 있는 프로그램



## build
g++ -o iconv_practice iconv_practice.cpp



## exec
./iconv_practice




## exam

```
======== [UTF ====>  EUC] ===========

  [China] encoding change : UTF-8 => EUC  (系统)
		 UTF-8 => EUC-KR : ERROR 84 (Invalid or incomplete multibyte or wide character)
		 UTF-8 => EUC-CN : ϵͳ
		 UTF-8 => EUC-JP : ERROR 84 (Invalid or incomplete multibyte or wide character)
		 UTF-8 => SHIFT_JIS : ERROR 84 (Invalid or incomplete multibyte or wide character)
		 UTF-8 => LATIN1 : ERROR 84 (Invalid or incomplete multibyte or wide character)


  [Japan] encoding change : UTF-8 => EUC (高層マンション)
	 	UTF-8 => EUC-KR : ���ޫ󫷫��
	 	UTF-8 => EUC-CN : ERROR 84 (Invalid or incomplete multibyte or wide character)
	 	UTF-8 => EUC-JP : ���إޥ󥷥��
	 	UTF-8 => SHIFT_JIS : ���w�}���V����
		UTF-8 => LATIN1 : ERROR 84 (Invalid or incomplete multibyte or wide character)


  [Korea] encoding change : UTF-8 => EUC (테스트2)
	 	UTF-8 => EUC-KR : �׽�Ʈ2
	 	UTF-8 => EUC-CN : ERROR 84 (Invalid or incomplete multibyte or wide character)
	 	UTF-8 => EUC-JP : ERROR 84 (Invalid or incomplete multibyte or wide character)
	 	UTF-8 => SHIFT_JIS : ERROR 84 (Invalid or incomplete multibyte or wide character)
	 	UTF-8 => LATIN1 : ERROR 84 (Invalid or incomplete multibyte or wide character)


======== [EUC ====>  UTF] ===========

  [China] encoding change : EUC => UTF-8  (系统)
	 	EUC-CN => UTF-8 : 系统
	 	EUC-KR => UTF-8 : 溝固
		EUC-JP => UTF-8 : 狼由
		SHIFT_JIS => UTF-8 : ERROR 7 (Argument list too long)
	 	LATIN1 => UTF-8 : ÏµÍ³


  [Japan] encoding change : EUC => UTF-8 (テム)
	 	EUC-CN => UTF-8 : ERROR 84 (Invalid or incomplete multibyte or wide character)
	 	EUC-KR => UTF-8 : e
	 	EUC-JP => UTF-8 : e
		SHIFT_JIS => UTF-8 : テム
		LATIN1 => UTF-8 : e


  [Korea] encoding change : EUC => UTF-8 (테스트)
		EUC-CN => UTF-8 : 抛胶飘
	 	EUC-KR => UTF-8 : 테스트
		EUC-JP => UTF-8 : 砺什闘
		SHIFT_JIS => UTF-8 : ERROR 7 (Argument list too long)
	 	LATIN1 => UTF-8 : Å×½ºÆ®
```
