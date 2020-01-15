# skripsi-sample
Deteksi mata uang asli dan palsu menggunakan Tensorflow

# Proses Pre-Processing pada gambar
Resize gambar
```
index_resize.py
```

Convert dataset meta labels xml to csv
```
python xml_For_csv.py
```

Convert csv dataset labels to TFRecord file format
```
python tfrecord.py --type=train --csv_input=data/trainlabels.csv  --output_path=data/train.record
python tfrecord.py --type=test --csv_input=data/testlabels.csv  --output_path=data/test.record
```

# Simpan di directory training untuk pemodelan
```
wget http://download.tensorflow.org/models/object_detection/ssd_mobilenet_v1_coco_2018_01_28.tar.gz

```
atau bisa (http://download.tensorflow.org/models/object_detection/ssd_mobilenet_v1_coco_2018_01_28.tar.gz)[clik aja]

# Setting Konfigurasi model dan class pada object
