# Analisis-Trend-Kualitas-Udara

Konsentrasi kualitas udara dengan data harian dianalisis menggunakan Mann- Kendall test dengan lokasi sembilan kota di Pulau Jawa. Pada contoh kali ini menggunakan lokasi Kota Depok. Analisa data menggunakan bantuan Jupyter Notebook dengan berbagai packages seperti numpy, pandas , pymannkendall, matplotlib.pyplot dan statsmodels.api. Waktu yang digunakan dalam analisa ini selama dua tahun

Hasil analisa data menggunakan Mann Kendall Test  dengan tingkat signifikansi 95%. Pada Mann Kendall Test, s dan z dipertimbangkan untuk mengidentifikasi kenaikan atau penurunan tren pada data time series parameter kualitas udara. Hasil tren dikatakan signifikan jika p  value < 0.05 (tingkat signifikansi 5%), tren dikatakan positif jika memiliki nilai z > 0 dan dikatakan negatif jika memiliki nilai z < 0. Sebelum dilakukan analisa data menggunakan Mann Kendall, hal yang perlu dilakukan adalah menguji stasioneritas dari data time series. Uji stasioneritas dapat menggunakan plot autocorrelation function (ACF). Dari Plot ACF dapat dikatakan signifikan jika lag pada plot ACF berada diluar pita biru. Nilai positif autokorelasi lag-1 akan menyebabkan nilai signifikansi tren overestimate, baik tren positif maupun negatif (Yue, dkk., 2002).

Software : jupyter notebook

Kemampuan yang digunakan : analisa statistic menggunakan python

Data : Konsentrasi NO2 menggunakan Sentinel 5P perekaman 2019-2020 yang diolah dengan GEE

Daftar Pustaka : 
Yue, Sheng., Pilon, P., Phinney, B., dan Cavadias, G.2002. The Influence of Autocorrelation
on the Ability to Detect Trend in Hydrological Series. Hydrological Processes. 16:
1807-1829
