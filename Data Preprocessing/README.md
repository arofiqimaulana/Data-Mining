# Data Preprocessing

## Pengertian
Data preprocessing merupakan sekumpulan teknik yang diterapkan pada database untuk menghapus noise missing value, dan data yang tidak konsisten. Dapat dikatakan bahwa 80% pekerjaan data science/data mining itu adalah di Data Preprocessing.  

## Jenis
### 1. Data Cleaning
Sebuah data tikatakan tidak bersih jika mengandung kotoran yang berupa **nilai kosonng** atau **pencilan** atau **inkonsistensi**. Beberapa teknik yang digunakan di [Data Cleaning](https://github.com/arofiqimaulana/Course-Python-For-Data-Analysis/tree/762d8c9c29ec0d12251c0268bd85f3c6c0b3ae24) adalah

- Mengisi missing values
- Menghaluskan/menghilangkan pencilan 
- memperbaiki inkonsistensi (misal perbedaan satuan)

### 2. Data Integration
Pada umumnya data yang ada tersebar di berbagai macam sumber seperti spreadsheet, MySQL, API. Sehingga terdapat kebutuhan untuk menggabungkan data tersebut menjadi satu kesatuan agar mudah dilakukan analisis data. Beberapa teknik yang digunakan di [Data Integration](ttps://github.com/arofiqimaulana/Course-Python-For-Data-Analysis/tree/762d8c9c29ec0d12251c0268bd85f3c6c0b3ae24) adalah
- menggunakan join pada MySQL
- menggunakan pd.merge di python
- menggunakan platform ETL seperti Pentaho, Talend, Airflow, Jupyter NB, dan lainnya. 

### 3. Data Reduction
Seringkali kita mempunyai dimensi data yang sangat besar (misal 100 variabel) yang menyebabkan proses analisis menjadi lama dan berat. 

Oleh karena itu diperlukan cara untuk mereduksi dimensi tersebut (misal menjadi 30 variabel). Namun dengan catatan 30 variabel tersebut mewakili sebagian informasi 50 variabel itu.

cara yang bisa digunakan adalah
1. Dimensionality Reduction (misal [PCA](https://github.com/arofiqimaulana/Artificial-Intelligence/tree/master/Unsupervised%20Learning/PCA)) 
2. Data Cube Aggregation
3. Data Compression
4. Numerosity Reduction
5. Discretization & Concept Hierarchy Operation

### 4. Data Normalization
Seringkali data yang kita punya perlu diubah ke dalam bentuk lainnya karena perbedaan satuan. Pada umumnya, [Normalisasi](https://github.com/arofiqimaulana/Artificial-Intelligence/blob/master/Unsupervised%20Learning/K-Mean/K-Mean%20using%20Python/clustering%20iris%20data.ipynb) digunakan saat proses Clustering. Beberapa teknik yang bisa digunakan adalah
- Tranformasi min-max
- Transformasi Z Score
- Transformasi penskalaan desimal 

### 5. Data Discretization
Seringkali data yang kita punya perlu diubah dari numerik ke kategorik maupun sebelumnya. Biasanya hal ini kita terapkan saat menggunakan Decision Tree agar lebih mudah menginterpretasikan rulesnya. Misal umur yang awalnya berupa variabel numerik diubah ke variabel kategorik menjadi remaja,dewasa, tua. Beberapa teknik [Data Discreatization](ttps://github.com/arofiqimaulana/Course-Python-For-Data-Analysis/tree/762d8c9c29ec0d12251c0268bd85f3c6c0b3ae24) yang bisa digunakan adalah
- bining
- histogram
- aturan sturgess

## Reference
- Suyanto. 2018. Machine Learning Tingkat Dasar dan Lanjut. Informatika. Bandung.