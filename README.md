# key-templates
Code/tricks done that can be used as templates


# Pandas:

I want to....

 ## Group a dataframe
 * solution: used pivot
 
 pivoted_df = df.pivot(index="Something like data_source_code", columns ="something like job_id", values = "something like revenue", aggfunc=np.sum)
 
 ## Get only the elements that are unique to each table
 
* solution: used the merge indicator

  df = pg_table.merge(netflix_df2, how = 'outer', on ='title', indicator = True)

  the indicator will say right only / left only and then we can pic elements that are based on the indicator under the merge column
  right_only_df = df[df['_merge']=='right_only']


 
 
 
