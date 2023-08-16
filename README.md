# Dataset-Throughput-Prediction

## Training
Diperuntukan untuk proses training LSTM, ARIMA, maupun SES

`
dataSheetType3.txt
`
Logging data pada Server Raspi 4 setiap menerima data dari ESP32 client.

Format Data:
```
File Size ; waktu menerima block pertama (sec) ; waktu menerima block pertama (m Sec) ; waktu menerima block terakhir (sec) ; waktu menerima block terakhir (m Sec) ;
```
`
dataSheetType3-V6-5s.csv
`
Data sheet yang sudah dirata ratakan setiap 5 detik sekali.

Format data:
```
ntp time , Throughput
```
## main-sistem
Data yang diperoleh saat main sistem dijalankan. Sudah menggunakan Throughput Prediction dan File Size Estimator

```
tp-final-1.txt = data Log Throughput Device 1 
pr-final-1.txt = data Log Prediction Device 1   
tp-final-2.txt = data Log Throughput Device 2
pr-final-2.txt = data Log Prediction Device 2
tp-final-3.txt = data Log Throughput Device 3
pr-final-3.txt = data Log Prediction Device 3
```

Format data Log Throughput:  
```
File Size ; waktu menerima block pertama (sec) ; waktu menerima block pertama (m Sec) ; waktu menerima block terakhir (sec) ; waktu menerima block terakhir (m Sec) ;
```
Format data Log Prediction:  
```
ntp time ; Prediksi
```