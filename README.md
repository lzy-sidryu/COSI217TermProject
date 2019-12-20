## Brief Code Structure

`CRF` contains the CRF suite training code, which is re-structured from hw3, 4 and 5. crf.ipynb contains the actual executed code, including the code generating input for BERT model. Input files for BERT are under bert_data sub-directory.

`BERT-NER` contains the BERT NER model forked and modified from the BERT-NER pytorch open source repo. The model is train and tested using the following command:

```
python run_ner.py --data_dir=esports_data/ --bert_model=bert-base-cased --output_dir=out_esports --max_seq_length=128 --do_train --num_train_epochs 5 --train_batch_size 16 --do_eval --eval_on test
```