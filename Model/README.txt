จะมีไฟล์ทั้งหมดที่เกี่ยวข้องกับโมเดลโดยจะแบ่งเป็น 3 ส่วน คือ โฟลเดอร์ “Model English”, โฟลเดอร์ “Model Thai” และ โฟลเดอร์ “util”
1.โฟลเดอร์ “Model English” 
จะมีไฟล์ทั้งหมดที่เกี่ยวข้องกับโมเดลภาษาอังกฤษโดยจะแบ่งเป็น 4 ส่วน คือ โฟลเดอร์ “Code_EnglishModel”, โฟลเดอร์ “Dataset”, โฟลเดอร์ “Model NLPAug” และ โฟลเดอร์ “Model Textattack”
1.1 โฟลเดอร์ “Code_EnglishModel” จะมีไฟล์โค้ดของโมเดลภาษาอังกฤษ โดยจะมีไฟล์ดังนี้
1.1.1 ไฟล์ “Augment_NLPAug_Wordembedding_Embedding.ipynb”                                            
คือ ไฟล์โค้ดโมเดลภาษาอังกฤษที่ใช้ Data Augmentation ด้วย NLPAug Library และ Word Embedding ด้วย Embedding Layer แบบ ทั่วไป โดยต้องมีการใช้ไฟล์เพื่อใช้ในการรันโค้ด ดังนี้ 						
- ไฟล์ “dataset_kaggle.csv”										
- ไฟล์ “dataset_research.csv”   									
- ไฟล์ “dataeng_text.csv”										
- ไฟล์ “nlp_finaldata”											
- ไฟล์ “_utils.ipnyb”											
- ไฟล์ “nlp_bilstm_emm.tflite”									
- ไฟล์ “nlp_cnn_emm.tflite”										
- ไฟล์ “nlp_gru_emm.tflite”										
- ไฟล์ “nlp_lstm_emm.tflite” 										
- ไฟล์ “nlp_rnn_emm.tflite”
1.1.2 ไฟล์ “Augment_NLPAug_Wordembedding_W2V.ipynb”  	                                     
คือ ไฟล์โค้ดโมเดลภาษาอังกฤษที่ใช้ Data Augmentation ด้วย NLPAug Library และ Word Embedding ด้วย Word2Vec โดยต้องมีการใช้ไฟล์เพื่อใช้ในการรันโค้ด ดังนี้ 			
- ไฟล์ “dataset_kaggle.csv”										
- ไฟล์ “dataset_research.csv”   									
- ไฟล์ “dataeng_text.csv”										
- ไฟล์ “nlp_finaldata”											
- ไฟล์ “_utils.ipnyb”											
- ไฟล์ “nlp_bilstm_w2v.tflite”										
- ไฟล์ “nlp_cnn_w2v.tflite”										
- ไฟล์ “nlp_gru_w2v.tflite”										
- ไฟล์ “nlp_lstm_w2v.tflite” 										
- ไฟล์ “nlp_rnn_w2v.tflite”
1.1.3 ไฟล์ “Augment_Textattack_Wordembedding_Embedding.ipynb”                                       
คือ ไฟล์โค้ดโมเดลภาษาอังกฤษที่ใช้ Data Augmentation ด้วย Textattack Library และ Word Embedding ด้วย Embedding Layer แบบทั่วไป โดยต้องมีการใช้ไฟล์เพื่อใช้ในการรันโค้ด ดังนี้ 						
- ไฟล์ “dataset_kaggle.csv”										
- ไฟล์ “dataset_research.csv”   									
- ไฟล์ “dataeng_text.csv”										
- ไฟล์ “ta_finaldata”											
- ไฟล์ “_utils.ipnyb”											
- ไฟล์ “ta_bilstm_emm.tflite”										
- ไฟล์ “ta_cnn_emm.tflite”										
- ไฟล์ “ta_gru_emm.tflite”										
- ไฟล์ “ta_lstm_emm.tflite” 										
- ไฟล์ “ta_rnn_emm.tflite”
1.1.4 ไฟล์ “Augment_Textattack_Wordembedding_W2V.ipynb”  	                                                
คือ ไฟล์โค้ดโมเดลภาษาอังกฤษที่ใช้ Data Augmentation ด้วย Textattack Library และ Word Embedding ด้วย Word2Vec โดยต้องมีการใช้ไฟล์เพื่อใช้ในการรันโค้ด ดังนี้ 		
- ไฟล์ “dataset_kaggle.csv”										
- ไฟล์ “dataset_research.csv”   									
- ไฟล์ “dataeng_text.csv”										
- ไฟล์ “ta_finaldata”											
- ไฟล์ “_utils.ipnyb”											
- ไฟล์ “ta_bilstm_w2v.tflite”										
- ไฟล์ “ta_cnn_w2v.tflite”										
- ไฟล์ “ta_gru_w2v.tflite”										
- ไฟล์ “ta_lstm_w2v.tflite” 										
- ไฟล์ “ta_rnn_w2v.tflite”

1.2 โฟลเดอร์ “Dataset” จะมีไฟล์ชุดข้อมูลที่ใช้ในโมเดลภาษาอังกฤษ โดยจะมีไฟล์ดังนี้		
1.2.1 ไฟล์ “dataeng_text.csv” คือไฟล์ชุดข้อมูลที่ใช้ในการตรวจสอบไฟล์โมเดลว่าสามารถทำงานได้ปกติได้หรือไม่												
1.2.2 ไฟล์ “dataset_kaggle.csv” คือไฟล์ชุดข้อมูลที่ใช้สร้างโมเดลที่มาจาก Kaggle			
1.2.3 ไฟล์ “dataset_research.csv” คือไฟล์ชุดข้อมูลที่ใช้สร้างโมเดลที่มาจากงานวิจัย		
1.2.4 ไฟล์ “nlp_finaldata.csv” คือไฟล์ชุดข้อมูลที่ได้ทำ Data Preprocessing และมีการทำ Data Augmentation ด้วย NLPAug Library					
1.2.5 ไฟล์ “ta_finaldata.csv” คือไฟล์ชุดข้อมูลที่ได้ทำ Data Preprocessing และมีการทำ Data Augmentation ด้วย Textattack Library					
1.2.6 ไฟล์ “nlp_emm_text_classification_vocab.txt”, ไฟล์ “nlp_w2v_text_classification_vocab.txt”, ไฟล์ “ta_emm_text_classification_vocab.txt” และไฟล์ “ta_w2v_text_classification_vocab.txt” ไฟล์เหล่านี้ คือ ไฟล์คลังคำศัพท์ (vocabulary) ของชุดข้อมูล

1.3 โฟลเดอร์ “Model NLPAug” จะมีไฟล์โมเดลภาษาอังกฤษทั้งหมดที่ใช้ Data Augmentation ด้วย NLPAug Library โดยจะมีโฟลเดอร์ 2 ส่วน คือ โฟลเดอร์ “Embedding” ซึ่งจะใช้ Word Embedding ด้วย Embedding Layer แบบทั่วไป และโฟลเดอร์ “W2V” ซึ่งจะใช้ Word Embedding ด้วย Word2Vec
1.4 โฟลเดอร์ “Model Textattack” จะมีไฟล์โมเดลภาษาอังกฤษทั้งหมดที่ใช้ Data Augmentation ด้วย Textattack Library โดยจะมีโฟลเดอร์ 2 ส่วน คือ โฟลเดอร์ “Embedding” ซึ่งจะใช้ Word Embedding ด้วย Embedding Layer แบบทั่วไป และโฟลเดอร์ “W2V” ซึ่งจะใช้ Word Embedding ด้วย Word2Vec

2. โฟลเดอร์ “Model Thai”
จะมีไฟล์ทั้งหมดที่เกี่ยวข้องกับโมเดลภาษาไทยโดยจะแบ่งเป็น 4 ส่วน คือ โฟลเดอร์ “Code_ThaiModel”, โฟลเดอร์ “Dataset”, โฟลเดอร์ “Model GridSearch” และ โฟลเดอร์ “Model WangchanBERTa”

2.1 โฟลเดอร์ “Code_ThaiModel” จะมีไฟล์โค้ดของโมเดลภาษาไทย โดยจะมีไฟล์ดังนี้		
2.1.1 ไฟล์ “Data_Preprocessing_Word_Segmentation.ipnyb”	                                       
คือ ไฟล์โค้ดที่ใช้ Tokenize ข้อความของชุดข้อมูลโดยต้องมีการใช้ไฟล์เพื่อใช้ในการรันโค้ด ดังนี้					
- ไฟล์ “smsfraud.xlsx”											
- ไฟล์ “smsnormal.xlsx”							
2.1.2 ไฟล์ “ThaiModel_Gridsearch.ipnyb” 					                                           
คือ ไฟล์โค้ดโมเดลภาษาไทยที่ใช้วิธีการ GridSearch โดยต้องมีการใช้ไฟล์เพื่อใช้ในการรันโค้ด ดังนี้ 				
- ไฟล์ “THFraud.txt”											
- ไฟล์ “THHam.txt”	             									
- ไฟล์ “final_data_th.csv”										
- ไฟล์ “exported_test_data.csv”									
- ไฟล์ “_utils.ipnyb”											
- ไฟล์ “thbilstm_grid.tflite”										
- ไฟล์ “thgru_grid.tflite”										
- ไฟล์ “thlstm_grid.tflite”										
- ไฟล์ “thrnn_grid.tflite”							
2.1.3 ไฟล์ “ThaiModel_WangchanBERTa.ipnyb”	                                                                            
คือ ไฟล์โค้ดโมเดลภาษาไทยที่ใช้ WangchanBERTa โดยต้องมีการใช้ไฟล์เพื่อใช้ในการรันโค้ด ดังนี้ 				
- ไฟล์ “THFraud.txt”											
- ไฟล์ “THHam.txt”	             									
- ไฟล์ “final_data_th.csv”										
- ไฟล์ “exported_test_data.txt”
		
2.2 โฟลเดอร์ “Dataset” คือ ไฟล์ชุดข้อมูลที่ใช้ในโมเดลภาษาไทย โดยจะมี 3 โฟลเดอร์ ดังนี้		
2.2.1 โฟลเดอร์ “data test” จะมีไฟล์ชุดข้อมูลที่ใช้ในการตรวจสอบไฟล์โมเดลว่าสามารถทำงานได้ปกติได้หรือไม่												
2.2.2 โฟลเดอร์ “dataset final” จะมีไฟล์ที่ได้จากการรวมชุดข้อมูล และไฟล์คลังคำศัพท์ (vocabulary) ของชุดข้อมูล โดยจะมีดังนี้									
- ไฟล์ “fraud_aug.txt” คือไฟล์ชุดข้อมูลของข้อความ SMS หลอกลวงที่ได้มีการทำ Data Augmentation												
- ไฟล์ “ham_aug.txt” คือไฟล์ชุดข้อมูลของข้อความ SMS ทั่วไปที่ได้มีการทำ Data Augmentation	
- ไฟล์ “merged_data.csv” คือไฟล์ชุดข้อมูลทั้งหมดที่ได้ผ่านการ Data Augmentation		
- ไฟล์ “final_data_th.csv” คือไฟล์ชุดข้อมูลทั้งหมดที่ได้ผ่านการ Data Preprocessing เพื่อนำไปใช้สร้างโมเดล													
- ไฟล์ “thai_text_classification_vocab.txt” คือ ไฟล์คลังคำศัพท์ (vocabulary) ของชุดข้อมูล
2.2.3 โฟลเดอร์ “OriginalData” จะมีไฟล์ชุดข้อมูลต้นฉบับและไฟล์ชุดข้อมูลที่ทำการ Tokenize แล้ว โดยจะมีไฟล์ ดังนี้ 												
- ไฟล์ “smsfraud.xlsx” คือไฟล์ชุดข้อมูลต้นฉบับของข้อความ SMS หลอกลวง				
- ไฟล์ “smsnormal.xlsx” คือไฟล์ชุดข้อมูลต้นฉบับของข้อความ SMS ทั่วไป					
- ไฟล์ “THFraud.txt” คือไฟล์ชุดข้อมูลของข้อความ SMS หลอกลวงที่ทำการ Tokenize แล้ว			
- ไฟล์ “THHam.txt” คือไฟล์ชุดข้อมูลของข้อความ SMS ทั่วไปที่ทำการ Tokenize แล้ว	

2.3 โฟลเดอร์ “Model GridSearch” จะมีไฟล์โมเดลภาษาไทยทั้งหมดที่ใช้วิธีการ GridSearch

2.4 โฟลเดอร์ “Model WangchanBERTa” จะมีไฟล์โมเดลภาษาไทยที่ใช้โมเดล WangchanBERTa

3. โฟลเดอร์ “util” 											
จะมีไฟล์สคริปต์ที่ใช้สำหรับดูกราฟ Train and Validation accuracy และ Train and Validation Loss
