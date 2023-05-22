# New_York_City_TLC_Tri_Record

## Latar Belakang

Perusahaan VeriFone Inc.bergerak di bidang layanan jasa taxi di Newyork City. Memiliki data 'New York City TLC Trip Record' dimana data berisi data setiap trip taxi dari perusahaan tersebut

Stackholder yang mengambil keputusan disini adalah Manajer Perusahaan Taxi VeriFone Inc.

## Permasalahan
Perusahaan ini ingin meningkatkan profit perusahaan dengan mengecek data 'New York City TLC Trip Record'.

Setelah dilihat dari data ternyata **ada permasalahan efesiensi lokasi pick up customer.**

Sebagai Data Analyst, kita akan mencoba menjawab pertanyaan berikut :

**Bagaimana cara meningkatkan profit perusahaan dan meningkatkan efesiensi lokasi pick up customer**

## Link Tableau [di sini](https://public.tableau.com/shared/FQ4HQPZPC?:display_count=n&:origin=viz_share_link)
## Link Persentasi [di sini](https://www.canva.com/design/DAFikSDd6k8/-fn16g1wcsT84yQ3qqXopg/edit?utm_content=DAFikSDd6k8&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)

## Data 

Dataset dapat diakses [di sini](https://drive.google.com/drive/folders/1NYHIL-RgVPW-HONz4pdzlcbIChF-c37N). 

1.	**VendorID** =  vendor atau perusahaan yang memiliki aplikasi taxi

2.	**lpep_pickup_datetime** = waktu pickup customer

3.	**lpep_dropoff_datetime** = waktu drop customer

4.	**store_and_fwd_flag** = 
- Y: Menunjukkan bahwa catatan perjalanan disimpan di memori kendaraan dan dikirim ke server kemudian (yaitu, perjalanan dengan metode "store and forward").
- N: Menunjukkan bahwa catatan perjalanan dikirim langsung ke server tanpa disimpan terlebih dahulu di memori kendaraan (yaitu, bukan perjalanan dengan metode "store and forward").

5.	**RatecodeID** = 
    - (1)	Standard rate (Tarif standar)
    - (2)	JFK (Kode tarif untuk perjalanan dari atau ke Bandara Internasional John F. Kennedy)
    - (3)	Newark (Kode tarif untuk perjalanan dari atau ke Bandara Internasional Newark Liberty)
    - (4)	Nassau or Westchester (Kode tarif untuk perjalanan ke Nassau atau Westchester di New York)
    - (5)	Negotiated fare (Tarif yang ditawar)
    - (6)	Group ride (Perjalanan kelompok)

6.	**PULocationID** = Lokasi taxi pick up customer

7.	**DOLocationID** = Lokasi taxi drop out 

8.	**passenger_count** = jumblah penumpang

9.	**trip_distance** = jarak tempuh selama perjalanan taksi dalam satuan mil dihitung menggunakan taximeter selama perjalanan berlangsung.

10.	**fare_amount** = MTA (Metropolitan Transportation Authority) tax sebesar $0,50 yang dikenakan pada tarif taksi di suatu daerah. MTA tax ini secara otomatis akan dikenakan berdasarkan tarif yang diukur oleh meteran pada kendaraan taksi yang digunakan selama perjalanan.

    MTA adalah sebuah badan transportasi yang bertanggung jawab atas sistem transportasi umum di daerah metropolitan di Amerika Serikat, termasuk di kota New York. Pada sistem transportasi tersebut, MTA tax sebesar $0,50 akan ditambahkan secara otomatis pada tarif taksi yang dihitung berdasarkan tarif meteran. Dalam hal ini, MTA tax merupakan biaya tambahan yang harus dibayar oleh pelanggan sebagai kontribusi untuk membiayai layanan transportasi umum di daerah tersebut.
 
11.	**mta_tax** = MTA tax adalah sebuah biaya tambahan yang dikenakan untuk mendukung layanan transportasi umum di daerah Metropolitan New York. Biaya tambahan sebesar $0,50 ini dikenakan pada setiap perjalanan taksi yang dilakukan di kota New York.

13.	**tip_amount** = besaran tip yang diberikan oleh penumpang

14.	**tolls_amount** = total biaya toll yang dibayarkan

15.	**improvement_surcharge** = ada biaya tambahan sebesar $0,30 yang dikenakan pada perjalanan taksi yang dipesan melalui sistem hail (mengangkat tangan sebagai tanda untuk memanggil taksi) pada saat penumpang naik ke dalam taksi

16.	**total_amount** = jumlah total biaya yang dibebankan kepada penumpang selama perjalanan taksi, dan tidak termasuk tips

17.	**payment_type** = tipe pembayaran
    - 1 = Credit card
    - 2 = Cash
    - 3 = No charge
    - 4 = Dispute
    - 5 = Unknown
    - 6 = Voided trip

18.	**trip_type** = 
    - 1 =  taksi dilakukan melalui penjemputan langsung (street hail), yaitu ketika penumpang menunjukkan minat untuk naik taksi dan pengemudi menyetujui untuk mengangkut mereka. 
    - 2 =  taksi dilakukan melalui panggilan dari pusat pengiriman taksi (dispatch), yaitu ketika penumpang memesan taksi melalui layanan panggilan atau aplikasi pemesanan taksi, dan pengemudi dipanggil untuk menjemput mereka.
