# Clustering
Teknik ini bertujuan untuk mengelompokkan objek-objek ke dalam suatu group yang memiliki kemiripan yang sama.

## Algoritma
Beberapa teknik yang dapat digunakan di clustering adalah
1. [k-Mean](https://github.com/arofiqimaulana/Artificial-Intelligence/tree/master/Unsupervised%20Learning/K-Mean)
2. [k-Medoids](https://github.com/arofiqimaulana/Artificial-Intelligence/tree/master/Unsupervised%20Learning/K-Medoids)
3. [Hierarcical Clustering (average linkage,single linkage,complete linkage,ward)](https://github.com/arofiqimaulana/Artificial-Intelligence/tree/master/Unsupervised%20Learning/Hierarchical%20Clustering)
4. DBSCAN (Density-Based Spatial Clustering of Applications with Noise)

## Tahapan
1. Penentuan banyaknya clusters
2. Normalisasi data
3. Pembentukan cluster
4. Evaluasi model 

## Optimal Clusters
Penentuan banyaknya cluster yang optimal bisa menggunakan
1. opini expert
2. silhouette
3. Elbow

## Normalisasi Data
Untuk mengatasi permasalahan perbedaan satuan, maka digunakan normalisasi seperti
1. min max
2. z-score
3. discreatization
4. bining

## Perhitungan Jarak
Kedekatan antar objek diukur menggunakan jarak. Jika datanya numerik, maka perhitungan jarak bisa menggunakan
1. Euclidian 
2. Manhattan
3. Minkowski
4. Mahalanobis

Jika datanya kategorik, maka perhitungan jarak bisa menggunakan
1. cosine
2. jaccard's coefficient
3. rank
4. simple matching coefficient (SMC)

## Reference
- https://www.codecademy.com/article/normalization
- https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.StandardScaler.html