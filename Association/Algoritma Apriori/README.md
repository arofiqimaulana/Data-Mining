# Algoritma Apriori
Adalah


# Flow
1. Menetapkan nilai minimum *Support* dan *Confidence*. <br>
Support(A) = COUNT(A)/COUNT(*), Support(A,B) = (COUNT(A&B)/COUNT(*)) <br>
Confidence = P(B|A) = COUNT(A&B)/COUNT(A)
2. Menghitung frequensi tiap itemsets
3. Menghilangkan itemsets yang berada di bawah minimum *Support* 
4. Menghilangkan itemsets yang berada di bawah minimum *Confidence*
