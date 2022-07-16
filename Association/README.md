# Association Rule
Merupakan teknik data mining untuk menemukan hubungan antar data (disebut juga Market Basket Analysis).

## Algoritma
Terdapat dua macam algoritma yang dapat digunakan untuk menyelesaikan permasalahan association rules.
1. Algoritma Apriori
2. Algoritma Frequent Pattern Growth (FP Growth)

## Aplikasi
1. Apakah orang yang beli sabun juga membeli shampo dan pasta gigi ?
2. Orang yang menonton Film A, B apakah juga menonton film J,K ?

## Terms
- Apriori : menemukan kumpulan item yang sering menggunakan
- FP Growth :
- support :
- antecedents : Jika rule yang terbentuk adalah A -> B, maka A disebut antecedents
- consequents : Jika rule yang terbentuk adalah A -> B, maka B disebut consequents
- antecedent support :
- consequent support :
- support : menunjukkan h berapa kali item x muncul dalam basis data transaksi
- confidence : ukuran yang menunjukkan hubungan antar 2 item secara conditional
- lift : suatu ukuran untuk mengetahui kekuatan  aturan  asosisasi  (association  rule)  yang telah  terbentuk. Nilai  lift  ratio  biasanya  digunakan sebagai  penentu  apakah  aturan  asosiasi  valid  atau tidak  valid.  lift = (support(A→C)/(coverage(A)*coverage(C))) . nilai lift > 1 menunjukkan bahwa hubungan antara antecedent dan consequent lebih signifikan dibandingkan sendiri-sendiri.
- leverage : mirip dengan lift, namun yang dihitung adalah selisihnya yaitu leverage = (support(A→C)-(coverage(A)*coverage(C)))
- conviction : nilai yang tinggi berarti konsekuensinya sangat tergantung pada anteseden. Misalnya, dalam kasus skor Conviction sempurna, hasilnya menjadi 0 (karena 1 - 1) di mana skor Conviction didefinisikan sebagai 'inf'. Mirip dengan lift, jika item independen, keyakinannya adalah 1.

## Formula
- \text{confidence}(A\rightarrow C) = \frac{\text{support}(A\rightarrow C)}{\text{support}(A)}, \;\;\; \text{range: } [0, 1]
- \text{confidence}(A\rightarrow C) = \frac{\text{support}(A\rightarrow C)}{\text{support}(A)}, \;\;\; \text{range: } [0, 1]
- \text{confidence}(A\rightarrow C) = \frac{\text{support}(A\rightarrow C)}{\text{support}(A)}, \;\;\; \text{range: } [0, 1]
- \text{confidence}(A\rightarrow C) = \frac{\text{support}(A\rightarrow C)}{\text{support}(A)}, \;\;\; \text{range: } [0, 1]

## FAQ


## Reference
1. Learning Data Mining With Python
2. https://www.solver.com/xlminer/help/association-rules
3. https://www.researchgate.net/publication/309293730_PENERAPAN_METODE_ASSOCIATION_RULE_MENGGUNAKAN_ALGORITMA_APRIORI_PADA_SIMULASI_PREDIKSI_HUJAN_WILAYAH_KOTA_BANDUNG
4. https://support.bigml.com/hc/en-us/articles/207310225-What-is-the-difference-between-lift-and-leverage-
5. https://core.ac.uk/download/pdf/299901448.pdf
6. https://gohighbrow.com/association-rules/
7. http://rasbt.github.io/mlxtend/user_guide/frequent_patterns/association_rules/

