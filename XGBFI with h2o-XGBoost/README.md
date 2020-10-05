the xgbfi_txt.zip package, where I changed the content of the package XgbFeatureInteractions.exe  to  XgbFeatureInteractions.txt
re-zipped the content, which you can change the extension to exe before using it. Hopefully this will help you download the package without any issue. 
 
- follow these step:
*[Download mono](https://www.mono-project.com/download/stable/) for mac or linux 
*[for ubuntu] (https://linuxize.com/post/how-to-install-mono-on-ubuntu-20-04/#:~:text=mono%2Dcomplete%20is%20a%20meta,mono%20%2D%2Dversion)

##What is MONO

Mono is a platform for developing and running cross-platform applications . It is a free and open-source implementation of Microsoft’s .NET framework.
Thus, It  doesn't not need to have windows system to use this package. I was able to run on it my mac and was able to verify linux environment as well. 

download the attached zip file (xgbfi_txt.zip) 
then run unzip xgbfi_txt.zip && cd xgbfi 
run mv mv XgbFeatureInteractions.txt  XgbFeatureInteractions.exe
run mono XgbFeatureInteractions.exe 
​run python xgbfi_from_zip.py 
           
this package already had example: h2o xgboost model,  in it thus when you run python xgbfi_from_zip.py  it should write it in a XgbFeatureInteractions.xlsx documentation within that xgbfi folder  and it should contain all the information you need as similar to xgbfi library.