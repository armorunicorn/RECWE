# RECWE
##使用方法
```
recwe -train train_data.txt -output-word output_vec.txt -output-char char_vec.txt -size 200 -window 5 -sample 1e-4 -negative 10 -iter 100 -threads 8 -min-count 5 -alpha 0.025 -binary 0  -char2comp char2comp.txt -join-type 1 -pos-type 3 -average-sum 1
recce -train train_data.txt -output-word output_char_vec.txt -output-char comp_vec.txt -size 200 -window 5 -sample 1e-4 -negative 10 -iter 100 -threads 8 -min-count 5 -alpha 0.025 -binary 0  -char2comp char2comp.txt -join-type 1 -pos-type 3 -average-sum 1
```

##比较
```
python word_sim.py -s tran_240.txt -e word_vec.txt
```