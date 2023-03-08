# Usage

```sh
git clone https://github.com/davidhong1/awk-print-percentile.git && cd awk-print-percentile
```

```sh
cat test_data/test.txt | awk '{print $2}' | sort -n | uniq -c | awk -f cal.awk
```

Will Output:

```
static       costt            count         diffPre
P50           63             866             866
P66           74            1092             226
P80           96            1333             241
P85          110            1407              74
P90          158            1490              83
P95          214            1573              83
P98          304            1621              48
P99          423            1638              17
P100     1024330            1654              16
count total: 1654
average cost: 1946.83
variance cost: 1.89647e+09
```
