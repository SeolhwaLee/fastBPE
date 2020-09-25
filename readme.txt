# procedures

./fast getvocab samsum_merge.txt > samsum_vocab

# Learn codes
./fast learnbpe 30000 train.json > samsum_codes

# Apply codes to train
./fast applybpe train.30000.json train.json samsum_codes
