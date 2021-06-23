24 variables
34191 obs
missin = 14%

categorical = ['location','wind_dir9am','rain_today']
numeric = ['min_temp','max_temp','rainfall','wind_gust_dir','wind_gust_speed',
'wind_dir9am ']
ts = ['date',]

to_drop = ['id','evaporation','sunshine']

## random thoughts...
build some sort of sequential features with look back windows??

evaporation = 98% NULLS
sunshine = 98% NULLS
