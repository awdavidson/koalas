.. _api.dataframe:

=========
DataFrame
=========
.. currentmodule:: databricks.koalas

Constructor
-----------
.. autosummary::
   :toctree: api/

   DataFrame

Attributes and underlying data
------------------------------

.. autosummary::
   :toctree: api/

   DataFrame.index
   DataFrame.columns
   DataFrame.empty

.. autosummary::
   :toctree: api/

   DataFrame.dtypes
   DataFrame.shape
   DataFrame.axes
   DataFrame.ndim
   DataFrame.size
   DataFrame.select_dtypes
   DataFrame.values

Conversion
----------
.. autosummary::
   :toctree: api/

   DataFrame.copy
   DataFrame.isna
   DataFrame.astype
   DataFrame.isnull
   DataFrame.notna
   DataFrame.notnull
   DataFrame.pad
   DataFrame.bool

Indexing, iteration
-------------------
.. autosummary::
   :toctree: api/

   DataFrame.at
   DataFrame.iat
   DataFrame.head
   DataFrame.idxmax
   DataFrame.idxmin
   DataFrame.loc
   DataFrame.iloc
   DataFrame.items
   DataFrame.iteritems
   DataFrame.iterrows
   DataFrame.itertuples
   DataFrame.keys
   DataFrame.pop
   DataFrame.tail
   DataFrame.xs
   DataFrame.get
   DataFrame.where
   DataFrame.mask
   DataFrame.query

Binary operator functions
-------------------------
.. autosummary::
   :toctree: api/

   DataFrame.add
   DataFrame.radd
   DataFrame.div
   DataFrame.rdiv
   DataFrame.truediv
   DataFrame.rtruediv
   DataFrame.mul
   DataFrame.rmul
   DataFrame.sub
   DataFrame.rsub
   DataFrame.pow
   DataFrame.rpow
   DataFrame.mod
   DataFrame.rmod
   DataFrame.floordiv
   DataFrame.rfloordiv
   DataFrame.lt
   DataFrame.gt
   DataFrame.le
   DataFrame.ge
   DataFrame.ne
   DataFrame.eq
   DataFrame.dot

Function application, GroupBy & Window
--------------------------------------
.. autosummary::
   :toctree: api/

   DataFrame.apply
   DataFrame.applymap
   DataFrame.pipe
   DataFrame.agg
   DataFrame.aggregate
   DataFrame.groupby
   DataFrame.rolling
   DataFrame.expanding
   DataFrame.transform
   DataFrame.map_in_pandas

.. _api.dataframe.stats:

Computations / Descriptive Stats
--------------------------------
.. autosummary::
   :toctree: api/

   DataFrame.abs
   DataFrame.all
   DataFrame.any
   DataFrame.clip
   DataFrame.corr
   DataFrame.count
   DataFrame.describe
   DataFrame.kurt
   DataFrame.kurtosis
   DataFrame.mad
   DataFrame.max
   DataFrame.mean
   DataFrame.min
   DataFrame.median
   DataFrame.pct_change
   DataFrame.prod
   DataFrame.product
   DataFrame.quantile
   DataFrame.nunique
   DataFrame.sem
   DataFrame.skew
   DataFrame.sum
   DataFrame.std
   DataFrame.var
   DataFrame.cummin
   DataFrame.cummax
   DataFrame.cumsum
   DataFrame.cumprod
   DataFrame.round
   DataFrame.diff
   DataFrame.eval

Reindexing / Selection / Label manipulation
-------------------------------------------
.. autosummary::
   :toctree: api/

   DataFrame.add_prefix
   DataFrame.add_suffix
   DataFrame.align
   DataFrame.between_time
   DataFrame.drop
   DataFrame.droplevel
   DataFrame.drop_duplicates
   DataFrame.duplicated
   DataFrame.equals
   DataFrame.filter
   DataFrame.head
   DataFrame.rename
   DataFrame.rename_axis
   DataFrame.reset_index
   DataFrame.set_index
   DataFrame.swapaxes
   DataFrame.swaplevel
   DataFrame.take
   DataFrame.isin
   DataFrame.sample
   DataFrame.truncate

.. _api.dataframe.missing:

Missing data handling
---------------------
.. autosummary::
   :toctree: api/

   DataFrame.backfill
   DataFrame.dropna
   DataFrame.fillna
   DataFrame.replace
   DataFrame.bfill
   DataFrame.ffill

Reshaping, sorting, transposing
-------------------------------
.. autosummary::
   :toctree: api/

   DataFrame.pivot_table
   DataFrame.pivot
   DataFrame.sort_index
   DataFrame.sort_values
   DataFrame.nlargest
   DataFrame.nsmallest
   DataFrame.stack
   DataFrame.unstack
   DataFrame.melt
   DataFrame.explode
   DataFrame.squeeze
   DataFrame.T
   DataFrame.transpose
   DataFrame.reindex
   DataFrame.reindex_like
   DataFrame.rank

Combining / joining / merging
-----------------------------
.. autosummary::
   :toctree: api/

   DataFrame.append
   DataFrame.assign
   DataFrame.merge
   DataFrame.join
   DataFrame.update
   DataFrame.insert

Time series-related
-------------------
.. autosummary::
   :toctree: api/

   DataFrame.shift
   DataFrame.first_valid_index
   DataFrame.last_valid_index

Serialization / IO / Conversion
-------------------------------
.. autosummary::
   :toctree: api/

   DataFrame.from_records
   DataFrame.info
   DataFrame.to_table
   DataFrame.to_delta
   DataFrame.to_parquet
   DataFrame.to_spark_io
   DataFrame.to_csv
   DataFrame.to_pandas
   DataFrame.to_html
   DataFrame.to_numpy
   DataFrame.to_koalas
   DataFrame.to_spark
   DataFrame.to_string
   DataFrame.to_json
   DataFrame.to_dict
   DataFrame.to_excel
   DataFrame.to_clipboard
   DataFrame.to_markdown
   DataFrame.to_records
   DataFrame.to_latex
   DataFrame.style

Spark-related
-------------
``DataFrame.spark`` provides features that does not exist in pandas but
in Spark. These can be accessed by ``DataFrame.spark.<function/property>``.

.. autosummary::
   :toctree: api/

   DataFrame.spark.schema
   DataFrame.spark.print_schema
   DataFrame.spark.frame
   DataFrame.spark.cache
   DataFrame.spark.persist
   DataFrame.spark.hint
   DataFrame.spark.to_table
   DataFrame.spark.to_spark_io
   DataFrame.spark.explain
   DataFrame.spark.apply
   DataFrame.spark.repartition
   DataFrame.spark.coalesce
   DataFrame.spark.checkpoint
   DataFrame.spark.local_checkpoint

.. _api.dataframe.plot:

Plotting
--------
``DataFrame.plot`` is both a callable method and a namespace attribute for
specific plotting methods of the form ``DataFrame.plot.<kind>``.

.. autosummary::
   :toctree: api/

   DataFrame.plot
   DataFrame.plot.area
   DataFrame.plot.barh
   DataFrame.plot.bar
   DataFrame.plot.hist
   DataFrame.plot.line
   DataFrame.plot.pie
   DataFrame.plot.scatter
   DataFrame.plot.density
   DataFrame.hist
   DataFrame.kde

Koalas-specific
---------------
``DataFrame.koalas`` provides Koalas-specific features that exists only in Koalas.
These can be accessed by ``DataFrame.koalas.<function/property>``.

.. autosummary::
   :toctree: api/

   DataFrame.koalas.attach_id_column
   DataFrame.koalas.apply_batch
   DataFrame.koalas.transform_batch
