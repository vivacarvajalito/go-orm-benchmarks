# Results

- orm-benchmark (with no flags)
```
Reports:

Insert
pgx:		4005	298530 ns/op	280 B/op	8 allocs/op
sqlc:		4203	299856 ns/op	280 B/op	8 allocs/op
beego:		4075	302104 ns/op	2401 B/op	56 allocs/op
gorp:		4239	303532 ns/op	1799 B/op	41 allocs/op
raw:		4077	308402 ns/op	704 B/op	13 allocs/op
ent:		3861	308714 ns/op	4150 B/op	97 allocs/op
pgx_pool:	4053	310204 ns/op	297 B/op	8 allocs/op
reform:		3847	315649 ns/op	1774 B/op	51 allocs/op
pg:		3950	317300 ns/op	1078 B/op	10 allocs/op
jet:		3696	319186 ns/op	3583 B/op	105 allocs/op
dbr:		3640	326567 ns/op	2688 B/op	65 allocs/op
sqlboiler:	3812	327355 ns/op	1591 B/op	34 allocs/op
sq:		3828	329580 ns/op	9777 B/op	100 allocs/op
bun:		3604	342810 ns/op	5028 B/op	13 allocs/op
gorm_prep:	3549	354920 ns/op	5192 B/op	65 allocs/op
gorm:		2932	379711 ns/op	7209 B/op	105 allocs/op
gen:		3144	380211 ns/op	10041 B/op	131 allocs/op
sqlx:		2467	470621 ns/op	856 B/op	19 allocs/op
rel:		2605	498336 ns/op	2639 B/op	45 allocs/op
godb:		2389	505588 ns/op	4537 B/op	115 allocs/op
zorm:		2390	514432 ns/op	5145 B/op	104 allocs/op
upper:		2378	520423 ns/op	5913 B/op	125 allocs/op
xorm:		2311	550094 ns/op	3121 B/op	88 allocs/op
pop:		1682	715470 ns/op	9454 B/op	234 allocs/op

InsertMulti
sqlc:		1560	741694 ns/op	66632 B/op	639 allocs/op
pgx_pool:	1605	753841 ns/op	47677 B/op	38 allocs/op
pgx:		1652	768076 ns/op	47746 B/op	38 allocs/op
raw:		1305	930570 ns/op	187134 B/op	930 allocs/op
beego:		1293	984165 ns/op	177706 B/op	2744 allocs/op
sq:		1267	992233 ns/op	237273 B/op	1706 allocs/op
reform:		1152	1056333 ns/op	462197 B/op	2746 allocs/op
gorm_prep:	1114	1112503 ns/op	254382 B/op	1890 allocs/op
ent:		1018	1170113 ns/op	396527 B/op	4597 allocs/op
pg:		896	1427831 ns/op	3315 B/op	112 allocs/op
jet:		874	1440021 ns/op	338336 B/op	6493 allocs/op
gorm:		831	1460336 ns/op	276184 B/op	5230 allocs/op
sqlx:		853	1463520 ns/op	170403 B/op	1550 allocs/op
bun:		694	1475613 ns/op	42587 B/op	219 allocs/op
gen:		828	1512382 ns/op	289369 B/op	5354 allocs/op
zorm:		636	1616030 ns/op	212125 B/op	2808 allocs/op
rel:		729	1670971 ns/op	312562 B/op	3265 allocs/op
upper:		716	1673549 ns/op	328153 B/op	4204 allocs/op
godb:		588	1768550 ns/op	260729 B/op	5894 allocs/op
xorm:		668	1788295 ns/op	258940 B/op	5518 allocs/op
pop:		bulk-insert is not supported
sqlboiler:	bulk-insert is not supported
gorp:		bulk-insert is not supported
dbr:		bulk-insert is not supported

Update
raw:		8498	148902 ns/op	750 B/op	13 allocs/op
sqlc:		7851	154410 ns/op	288 B/op	8 allocs/op
reform:		4239	296297 ns/op	1775 B/op	51 allocs/op
beego:		4068	300439 ns/op	1736 B/op	46 allocs/op
gorp:		4204	306547 ns/op	1205 B/op	32 allocs/op
ent:		4051	310206 ns/op	4726 B/op	98 allocs/op
sqlboiler:	3825	313087 ns/op	902 B/op	17 allocs/op
pgx_pool:	3816	319590 ns/op	305 B/op	8 allocs/op
dbr:		3915	325009 ns/op	2651 B/op	57 allocs/op
sqlx:		3691	326840 ns/op	872 B/op	20 allocs/op
sq:		4123	327236 ns/op	7415 B/op	90 allocs/op
pgx:		3871	327826 ns/op	288 B/op	8 allocs/op
jet:		3769	339372 ns/op	4566 B/op	126 allocs/op
pop:		3518	342678 ns/op	5856 B/op	184 allocs/op
gorm_prep:	3753	344243 ns/op	5072 B/op	56 allocs/op
pg:		3621	350118 ns/op	768 B/op	9 allocs/op
bun:		3490	363930 ns/op	4762 B/op	5 allocs/op
gorm:		3212	382139 ns/op	6832 B/op	99 allocs/op
gen:		2952	396681 ns/op	13408 B/op	161 allocs/op
zorm:		2326	512297 ns/op	4449 B/op	84 allocs/op
xorm:		2367	526126 ns/op	4305 B/op	145 allocs/op
rel:		2287	532496 ns/op	3048 B/op	45 allocs/op
godb:		2209	534556 ns/op	5145 B/op	154 allocs/op
upper:		982	1196313 ns/op	16733 B/op	390 allocs/op

Read
pgx:		8022	153921 ns/op	776 B/op	18 allocs/op
sqlc:		7862	154194 ns/op	904 B/op	19 allocs/op
pgx_pool:	7844	154433 ns/op	963 B/op	19 allocs/op
beego:		8142	161525 ns/op	2113 B/op	75 allocs/op
raw:		8085	161565 ns/op	2093 B/op	50 allocs/op
reform:		6961	168875 ns/op	3230 B/op	86 allocs/op
gorp:		7342	175811 ns/op	3909 B/op	194 allocs/op
pop:		7388	178896 ns/op	3212 B/op	66 allocs/op
ent:		6854	182315 ns/op	5684 B/op	145 allocs/op
rel:		6548	182727 ns/op	2336 B/op	47 allocs/op
sq:		7156	184827 ns/op	11159 B/op	135 allocs/op
dbr:		6222	185106 ns/op	2184 B/op	36 allocs/op
gorm_prep:	6780	185566 ns/op	4566 B/op	89 allocs/op
pg:		7150	185629 ns/op	872 B/op	20 allocs/op
sqlboiler:	6580	187871 ns/op	947 B/op	14 allocs/op
bun:		6988	188004 ns/op	5844 B/op	39 allocs/op
zorm:		6088	199930 ns/op	3337 B/op	74 allocs/op
jet:		5911	202487 ns/op	13067 B/op	273 allocs/op
gorm:		4957	229242 ns/op	4982 B/op	102 allocs/op
gen:		4816	250099 ns/op	10509 B/op	154 allocs/op
sqlx:		3606	335647 ns/op	2008 B/op	43 allocs/op
godb:		3681	356526 ns/op	4097 B/op	102 allocs/op
upper:		3367	357627 ns/op	5085 B/op	110 allocs/op
xorm:		3271	358523 ns/op	5162 B/op	131 allocs/op

ReadSlice
reform:		7461	170538 ns/op	4045 B/op	100 allocs/op
pgx:		4490	252470 ns/op	30320 B/op	513 allocs/op
pgx_pool:	4558	253210 ns/op	30379 B/op	513 allocs/op
sqlc:		4429	270329 ns/op	54624 B/op	620 allocs/op
raw:		3835	306373 ns/op	38373 B/op	1038 allocs/op
pg:		3417	349193 ns/op	23026 B/op	629 allocs/op
upper:		3450	369249 ns/op	4821 B/op	90 allocs/op
gorp:		3129	373322 ns/op	57543 B/op	1494 allocs/op
ent:		3112	379461 ns/op	77398 B/op	2036 allocs/op
sqlx:		3087	381348 ns/op	37512 B/op	1225 allocs/op
pop:		2980	395016 ns/op	76972 B/op	1306 allocs/op
sq:		2836	411206 ns/op	152500 B/op	1829 allocs/op
dbr:		2881	411558 ns/op	30944 B/op	1253 allocs/op
bun:		2704	424421 ns/op	34211 B/op	1124 allocs/op
beego:		2684	433792 ns/op	55350 B/op	3077 allocs/op
sqlboiler:	2517	464847 ns/op	67331 B/op	2260 allocs/op
gorm_prep:	2522	472634 ns/op	43529 B/op	2082 allocs/op
gorm:		2250	535719 ns/op	44747 B/op	2196 allocs/op
gen:		2004	564590 ns/op	50275 B/op	2248 allocs/op
zorm:		1962	591198 ns/op	169542 B/op	2959 allocs/op
xorm:		2014	599571 ns/op	121236 B/op	4407 allocs/op
jet:		1912	627298 ns/op	192700 B/op	3642 allocs/op
godb:		1772	675915 ns/op	75389 B/op	3084 allocs/op
rel:		1765	677194 ns/op	149042 B/op	2553 allocs/op
```
