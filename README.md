# pandas-challenge-1
Module 4 homework



2. Index(['first', 'last', 'job', 'phone', 'email', 'client_id', 'order_id',
       'order_date', 'order_week', 'order_year', 'item_id', 'category',
       'subcategory', 'unit_price', 'unit_cost', 'unit_weight', 'qty',
       'line_number'],
      dtype='object')


columnNames_df = pd.DataFrame(['first', 'last', 'job', 'phone', 'email', 'client_id', 'order_id',
       'order_date', 'order_week', 'order_year', 'item_id', 'category',
       'subcategory', 'unit_price', 'unit_cost', 'unit_weight', 'qty',
       'line_number'], dtype='object')
columnNames_df.head()


<class 'pandas.core.frame.DataFrame'>
RangeIndex: 54639 entries, 0 to 54638
Data columns (total 18 columns):
 #   Column       Non-Null Count  Dtype  
---  ------       --------------  -----  
 0   first        54639 non-null  object 
 1   last         54639 non-null  object 
 2   job          54639 non-null  object 
 3   phone        54639 non-null  object 
 4   email        54639 non-null  object 
 5   client_id    54639 non-null  int64  
 6   order_id     54639 non-null  int64  
 7   order_date   54639 non-null  object 
 8   order_week   54639 non-null  int64  
 9   order_year   54639 non-null  int64  
 10  item_id      54639 non-null  object 
 11  category     54639 non-null  object 
 12  subcategory  54639 non-null  object 
 13  unit_price   54639 non-null  float64
 14  unit_cost    54639 non-null  float64
 15  unit_weight  54639 non-null  float64
 16  qty          54639 non-null  int64  
 17  line_number  54639 non-null  int64  
dtypes: float64(3), int64(6), object(9)
memory usage: 7.5+ MB

df.value_counts()
mostEntries = {
    ['category'], ['qty']
}
df = pd.DataFrame(mostEntries)


subcategory
bathroom supplies    6424
Name: count, dtype: int64

7
client_id
33615    220
66037    211
46820    209
38378    207
24741    207
Name: count, dtype: int64

8
[33615, 66037, 46820, 38378, 24741]

9
64313


PART 2
10
unit_price	qty	line_subtotal
0	1096.80	105	115164.00
1	24.95	21	523.95

11
unit_price	unit_weight	qty	total_weight	shipping_price
0	1096.80	7.50	105	787.50	5512.50
1	24.95	1.49	21	31.29	312.90
2	13.52	1.68	39	65.52	458.64