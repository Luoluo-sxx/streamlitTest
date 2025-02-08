import streamlit as st
import pandas as pd
import numpy as np

st.write("hello world!")
df = pd.DataFrame(
    np.random.randn(10, 5),
    columns=('第%d列' % (i+1) for i in range(5))
)

st.table(df)
