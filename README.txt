CS784 Stage II

Group Members:
- Junwei Su
- Wuyue Liu
- Zhicheng Gu


Golden Data: step2_golden_data.txt

- Each product is represented in the JSON format, which is the same as the original file:

{"Brand": "", "Product ID": "", "Product Name": ""}

For example:
{"Brand": "EDGE", "Product ID": "42738783#TigerDirect", "Product Name": "EDGE - DDR3 - 4 GB - DIMM 240-pin - 1600 MHz / PC3-12800 - unbuffered - ECC"}

Development Set I: step2_training_set & step2_tuning_set
- This two set all together contribute to our development set
- In particular training_set_size = 160, tuning_set_size = 60

Test Set J: step2_testing_set
- The size of the testing set is 130

Code: Extractor
- step2.py  This is where we randomly sample 350 products from the set of 10K labeled product pairs.
- step3.py  Randomly split S into a development set I and a testing set J.
- step4_dic_builder.py  Where we build our dictionary.
- step4.py and step4_helper.py   Where we extract the brand and calculate the precision and recall. 