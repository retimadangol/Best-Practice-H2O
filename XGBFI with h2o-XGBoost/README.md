
## xgbfi.zip 
(which is the extraction of XGBFI library) to be used H2O-XGBoost

https://github.com/Far0n/xgbfi

## After you unzip it contents:
* example: h2o-xgboost model
* XgbFeatureInteractions.exe
* XgbFeatureInteractions.exe.config
* example: output for feature interaction level of the model XgbFeatureInteractions.xlsx
* lib
* xgbfi_from_zip.py

## How to use it:
follow these step:

* [Download mono](https://www.mono-project.com/download/stable/) for mac or linux

* [for ubuntu](https://linuxize.com/post/how-to-install-mono-on-ubuntu-20-04/#:~:text=mono%2Dcomplete%20is%20a%20meta,mono%20%2D%2Dversion)

* download the zip file (xgbfi.zip)
* then run ```unzip xgbfi.zip && cd xgbfi```
* run ```mono XgbFeatureInteractions.exe```
* run ```python xgbfi_from_zip.py```

## What is MONO

Mono is a platform for developing and running cross-platform applications . It is a free and open-source implementation of Microsoft’s .NET framework.
Thus, It  doesn't not need to have windows system to use this package. I was able to run on it my mac and was able to verify linux environment as well. 

### If you are not able to Download the folder due to exe file content uder linux then:

* Download xgbfi_txt.zip package

where I changed the content of the package XgbFeatureInteractions.exe  to  XgbFeatureInteractions.txt
re-zipped the content, which you can change the extension to exe before using it. Hopefully this will help you download the package without any issue. 

* download the zip file (xgbfi_txt.zip)
* then run ```unzip xgbfi_txt.zip && cd xgbfi```
* run ```mv XgbFeatureInteractions.txt  XgbFeatureInteractions.exe```
* run ```mono XgbFeatureInteractions.exe```
* run ```python xgbfi_from_zip.py``
 
