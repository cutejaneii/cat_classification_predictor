# cat_classification_predictor

### Train Model
python retrain.py \
  --image_dir=cat_photos \
  --bottleneck_dir=bottlenecks \
  --model_dir=inception \
  --learning_rate=0.5 \
  --summaries_dir=training_summaries/long \
  --output_graph=retrained_graph.pb \
  --output_labels=retrained_labels.txt
  
 We got the image_list as ['blue', 'eng short', 'black white', 'normal', 'black', 'orange', 'american short', 'white']
  
### Predict Cat Category
python label_image.py predict/white001.jpg

Result:

白貓 (score = 0.57062)
美短貓 (score = 0.19097)
虎斑貓 (score = 0.16022)
黑貓 (score = 0.05089)
賓士貓 (score = 0.01711)
藍貓 (score = 0.00437)
橘貓 (score = 0.00424)
英短貓 (score = 0.00159)



### Doc
可參考:https://ithelp.ithome.com.tw/articles/10189949
