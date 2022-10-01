# Association Rule
Suatu teknik dalam data mining yang berguna untuk menentukan aturan asosiatifantara kombinasi item disebut (Kusrini, Emha, 2009).

## Algoritma
Terdapat dua macam algoritma yang dapat digunakan untuk menyelesaikan permasalahan association rules.
1. Algoritma Apriori. <br>
Algoritma ini berbasis *array-based* yaitu men-generate berbagai kemungkinan kombinasi item menjadi kandidat-kandidat. Kandidat itulah nantinya yang akan diseleksi menjadi suatu aturan. Algoritma ini termasuk ke dalam breadth first search
2. Algoritma Frequent Pattern Growth (FP Growth). <br>
Algoritma ini tidak melakukan generate kombinasi item, namun menggunakan dataset original. Hal ini yang membedakan dengan algoritma apriori yang notabene men-generate semua kemungkinanan kandidat meskipun kandidat tersebut tidak ada di data aslinya. Oleh karena itu teknik ini akan lebih cepat dibandingkan apriori. Algoritma FP Growth ini termasuk depth first search algorithm.

## Aplikasi
1. Apakah orang yang beli sabun juga membeli shampo dan pasta gigi ?
2. Orang yang menonton Film A, B apakah juga menonton film J,K ?


## Reference
1. https://www.youtube.com/watch?v=qaTC0Y_evbk&ab_channel=UnfoldDataScience
