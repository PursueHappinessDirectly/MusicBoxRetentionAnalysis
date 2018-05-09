# MusicBoxRetentionAnalysis

The reading sequence is
0_create_data_folders.sh    
1_download_data.ipynb	    
2_unpack_and_clean_files.sh	    
3_etl_down_sample_by_user.ipynb	    
4_EDA_with_spark.ipynb       
5_feature_engineer_with_spark.ipynb      
6_train_model_sklearn.ipynb      

Summary of data analysis       
Part zero: create_data_folders.sh     
■ Create data folder for data downloading     

Part one: download_data.ipynb  
■ Down load data from AWS     

Part two: unpack_and_clean_files.sh    
■ Un-compress the downloaded data and combine them to each category.    

Part three: etl_down_sample_by_user.ipynb     
■ Removed the robots users from data set based on unusual music play frequency.     
■ Applied down sampling method to cut data size in half.     
■ Introduced the data structure and content.    

Part four: EDA_with_spark.ipynb      
Explored the following questions:           
■ What's the user activity from 04/01 to 05/12?     
■ What's the device distribution?      
■ What's the percentage of paid songs?      
■ Why do users stop playing songs before it ends?       
■ What's the weekly retention rate for users?      

Part five: feature_engineer_with_spark.ipynb      
■ Created and engineered features for retention analysis.      

Part six: train_model_sklearn.ipynb       
■ Based on generated feature, built logistic regression, random forest, GBDT and neural network to predict monthly retention behavior.     
■ Compared the performance of each model through cross-validation.     
■ Usd grid-search to fine tuning random forest model due to its good performance.     
