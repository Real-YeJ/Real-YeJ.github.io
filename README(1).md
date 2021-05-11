# ArT
ICDAR2019-ArT evaluation web：https://rrc.cvc.uab.es/  
How to evaluate your result:  
1. Register your account according to the instructions on the official website  
2. Convert the txt result to json result by using art_result_txt_2_json.py  
3. Select the ICDAR2019-ArT challenge to submit your json result  

# Total-Text & CTW-1500
Required python libraries: numpy, Polygon2. Evaluate your result, please run:  

    python script.py -g=gt.zip -s=result.zip
