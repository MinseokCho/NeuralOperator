NeuralOperator (ACML 2018)
==========================
This repository contains data and source code for the system described in:  
**Adversarial TableQA: Evaluation and Supervision for Question Answering on Tables**

Dataset
-------
An altered version of the original **WikiSQL dataset** (https://github.com/salesforce/WikiSQL), by transforming the SQL statements into "operand information".

Dataset Link
------------
https://drive.google.com/drive/folders/1qkxAEee0_Wm_2ohpbRYk_nvndiMBjEOp

Dataset Info
--------------
* Question data
	* Files  
		train_set.txt, dev_set.txt, test_set.txt (Tab-separated)  
	* Format  
		"table ID"	"operation"	"condition"	"question"	"operand information"	"answer"  
	* Notes  
		If an instance has more than one value, it is separated by ';'.  
		If there is no correct answer, "operand information" and "answer" are '-'.  

* Tables
	* json  
		* They are files of **WikiSQL**. Refer to its github page.
	* tsv  
		* filename.tsv / filename is the same as table ID.
		* tap-separated
		* First line is column headers in the table.
		