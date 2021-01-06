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
  
  
### Predict Cat Category
python predict.py predict/amer003.jpg

### Doc
可參考:https://ithelp.ithome.com.tw/articles/10189949
