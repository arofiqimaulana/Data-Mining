# Data Preprocessing

## Pengertian
Data preprocessing merupakan sekumpulan teknik yang diterapkan pada database untuk menghapus noise missing value, dan data yang tidak konsisten.

## Jenis
### 1. Data Cleaning
Seringkali data yang kita punya harus dibersihkan karena mengandung missing values, outlier, filtering, drop duplicates value. Beberapa perintah yang bisa digunakan

```
df.fillna('',inplace=True)
df.drop_duplicates(inplace=True)
df[df.status != '']

import re
rs_remove_characters = [re.sub(r'[^\w]', '', k) for k in rs_lower]
```
### 2. Data Transformation
Seringkali data yang kita punya perlu diubah ke dalam bentuk lainnya seperti normalization, pemilihan attribute, dan discretization. Beberapa perintah yang bisa digunakan seperti

```
from sklearn.preprocessing import StandardScaler

scaled_features = StandardScaler().fit_transform(X) # transform ke Z score
df['is_Anomaly'] = df.apply(getAnomaly,axis=1) # apply function
df = pd.get_dummies(df['billingcycle']) # create dummies
df['nomor'] = df['nomor'].astype('int') # convert str to int
``` 

### 3. Data Reduction
Seringkali kita mempunyai dimensi data yang sangat besar (misal 100 variabel) yang menyebabkan proses analisis menjadi lama dan berat. 

Oleh karena itu diperlukan cara untuk mereduksi dimensi tersebut (misal menjadi 30 variabel). Namun dengan catatan 30 variabel tersebut mewakili sebagian informasi 50 variabel itu.

cara yang bisa digunakan adalah
1. Dimensionality Reduction
2. Data Cube Aggregation: 
3. Data Compression
4. Numerosity Reduction
5. Discretization & Concept Hierarchy Operation

## Reference
- https://www.dqlab.id/langkah-awal-dalam-pemrosesan-data-dalam-data-mining 
- https://www.geeksforgeeks.org/data-reduction-in-data-mining/