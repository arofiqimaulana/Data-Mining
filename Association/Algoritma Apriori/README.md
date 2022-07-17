# Algoritma Apriori
Adalah teknik penemuan pola hubungan antar item menggunakan frequensi tiap item.

# Flow
1. Menetapkan nilai minimum *Support* dan *Confidence*. <br>
Support(A) = COUNT(A)/COUNT(*), Support(A,B) = (COUNT(A&B)/COUNT(*)) <br>
Confidence = P(B|A) = COUNT(A&B)/COUNT(A)
2. Menghitung frequensi tiap itemsets
3. Menghilangkan itemsets yang berada di bawah minimum *Support* 
4. Menghilangkan itemsets yang berada di bawah minimum *Confidence*

## Terms
- antecedents : Jika rule yang terbentuk adalah A -> B, maka A disebut antecedents
- consequents : Jika rule yang terbentuk adalah A -> B, maka B disebut consequents
- support : menunjukkan berapa kali suatu item muncul dalam basis data transaksi
- confidence : ukuran yang menunjukkan hubungan antar 2 item secara conditional
- lift : suatu ukuran untuk mengetahui kekuatan  aturan  asosisasi  (association  rule)  yang telah  terbentuk. Nilai  lift  ratio  biasanya  digunakan sebagai  penentu  apakah  aturan  asosiasi  valid  atau tidak  valid.  lift = (support(A→C)/(coverage(A)*coverage(C))) . nilai lift > 1 menunjukkan bahwa hubungan antara antecedent dan consequent lebih signifikan dibandingkan sendiri-sendiri.
- leverage : mirip dengan lift, namun yang dihitung adalah selisihnya yaitu leverage = (support(A→C)-(coverage(A)*coverage(C)))
- conviction : nilai yang tinggi berarti konsekuensinya sangat tergantung pada anteseden. Misalnya, dalam kasus skor Conviction sempurna, hasilnya menjadi 0 (karena 1 - 1) di mana skor Conviction didefinisikan sebagai 'inf'. Mirip dengan lift, jika item independen, keyakinannya adalah 1.

## Formula

#### Confidence
$$ \text{confidence}(A\rightarrow B) = \frac{\text{support}(A\rightarrow B)}{\text{support}(A)},  \text{range: } [0, 1] $$ <br>

#### Lift
$$ \text{lift}(A\rightarrow B) = \frac{\text{confidence}(A\rightarrow B)}{\text{support}(B)},  \text{range: } [0, \infty] $$ <br>

#### Leverage
$$ \text{leverage}(A\rightarrow B) = \text{support}(A\rightarrow B) - \text{support}(A) \times \text{support}(B), \text{range: } [-1, 1] $$ <br>

#### Conviction
$$ \text{conviction}(A\rightarrow B) = \frac{1 - \text{support}(B)}{1 - \text{confidence}(A\rightarrow B)}, \text{range: } [0, \infty] $$ 


## Reference
1. Learning Data Mining With Python
2. https://www.solver.com/xlminer/help/association-rules
3. https://www.researchgate.net/publication/309293730_PENERAPAN_METODE_ASSOCIATION_RULE_MENGGUNAKAN_ALGORITMA_APRIORI_PADA_SIMULASI_PREDIKSI_HUJAN_WILAYAH_KOTA_BANDUNG
4. https://support.bigml.com/hc/en-us/articles/207310225-What-is-the-difference-between-lift-and-leverage-
5. https://core.ac.uk/download/pdf/299901448.pdf
6. https://gohighbrow.com/association-rules/
7. http://rasbt.github.io/mlxtend/user_guide/frequent_patterns/association_rules/