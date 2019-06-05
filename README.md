## 简单介绍

这是一个使用bert网络，采用微调方式训练，训练一个复述对判别模型

python3 paraphrase_classifier.py \
    --task_name=classify   \
    --do_train=true   \
    --do_eval=true   \
    --data_dir=data/ \
    --vocab_file=results/BERT/chinese_L-12_H-768_A-12/vocab.txt \
    --bert_config_file=results/BERT/chinese_L-12_H-768_A-12/bert_config.json  \
    --init_checkpoint=results/BERT/chinese_L-12_H-768_A-12/bert_model.ckpt \
    --max_seq_length=150  \
    --train_batch_size=32   \
    --learning_rate=3e-5 \
    --num_train_epochs=10 \
    --output_dir=results/classify/

