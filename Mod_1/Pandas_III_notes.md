optional arguments are (\*args)

df['high_or_low'] = df.total_litres_of_pure_alcohol.map(lambda total : 'High' if total > df.total_litres_of_pure_alcohol.mean() else 'Low')

## is the same as

df['high_or_low'] = ['High' if total > df.total_litres_of_pure_alcohol.mean() else 'Low' for total in df.total_litres_of_pure_alcohol]
df

inplace argument

# groupby

"The method can be summarized as split-apply-combine"

it means to group by values in a column and then agregate them

groupby returns a DataFrameGroupBy object
