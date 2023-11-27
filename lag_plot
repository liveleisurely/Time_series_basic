import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
from pandas.plotting import lag_plot
from matplotlib.pyplot as plt
import koreanize_matplotlib

# 예제 데이터 생성
np.random.seed(42)
data = pd.Series(np.random.randn(1000), index=pd.date_range('2022-01-01', periods=1000))


# lag plot 그리기
lag_plot(data)
plt.title('Lag Plot 예제')
plt.show()

# 종속변수의 t시점 기준 lag별 관계도 확인
figure, axes = plt.subplots(1, 4, figsize=(30,5))
pd.plotting.lag_plot(data, lag=1, ax=axes[0])
pd.plotting.lag_plot(data, lag=5, ax=axes[1])
pd.plotting.lag_plot(data, lag=10, ax=axes[2])
pd.plotting.lag_plot(data, lag=50, ax=axes[3])
