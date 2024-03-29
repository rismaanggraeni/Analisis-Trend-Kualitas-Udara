# Analisis-Trend-Kualitas-Udara

Konsentrasi kualitas udara dengan data harian dianalisis menggunakan Mann- Kendall test dengan lokasi sembilan kota di Pulau Jawa. Pada contoh kali ini menggunakan lokasi Kota Depok. Analisa data menggunakan bantuan Jupyter Notebook dengan berbagai packages seperti numpy, pandas , pymannkendall, matplotlib.pyplot dan statsmodels.api. Waktu yang digunakan dalam analisa ini selama dua tahun

![trend_no2](https://user-images.githubusercontent.com/78722448/168215715-a4d97920-4380-453b-b20b-b591d5788d4d.jpg)
                              
                              Gambar 1 : Trend kualitas udara (NO2) 

Hasil analisa data menggunakan Mann Kendall Test  dengan tingkat signifikansi 95%. Pada Mann Kendall Test, s dan z dipertimbangkan untuk mengidentifikasi kenaikan atau penurunan tren pada data time series parameter kualitas udara. Hasil tren dikatakan signifikan jika p  value < 0.05 (tingkat signifikansi 5%), tren dikatakan positif jika memiliki nilai z > 0 dan dikatakan negatif jika memiliki nilai z < 0. Sebelum dilakukan analisa data menggunakan Mann Kendall, hal yang perlu dilakukan adalah menguji stasioneritas dari data time series. Uji stasioneritas dapat menggunakan plot autocorrelation function (ACF). Dari Plot ACF dapat dikatakan signifikan jika lag pada plot ACF berada diluar pita biru. Nilai positif autokorelasi lag-1 akan menyebabkan nilai signifikansi tren overestimate, baik tren positif maupun negatif (Yue, dkk., 2002).

![hasil_trend_no2](https://user-images.githubusercontent.com/78722448/168216628-487f1bb0-0b2a-4703-9d2e-01735a3f1683.jpg)
                          
                          Gambar 2 : Hasil uji trend menggunakan Mann Kendall Test

![acf_no2](https://user-images.githubusercontent.com/78722448/168216783-d2d0bb29-44f0-4395-baca-1b63dbde4c42.jpg)

                       Gambar 3 : plot autocorrelation function (ACF) konsentrasi NO2

Daftar Pustaka : 
Yue, Sheng., Pilon, P., Phinney, B., dan Cavadias, G.2002. The Influence of Autocorrelation
on the Ability to Detect Trend in Hydrological Series. Hydrological Processes. 16:
1807-1829
