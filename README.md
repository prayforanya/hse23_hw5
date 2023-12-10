# hse23_hw5
  
[Ссылка на Google Colab для первой части](https://colab.research.google.com/drive/1z6CV_MombkBE7I1q3H6WMxAI7AAlkE-h?usp=sharing)

# Нормализация

Данные сырые и их необходимо нормализовать, так как разница в экспрессии генов может быть обусловлена биологическими оссобеностями (длиной генов) или эксперементальными (чтений для какого-то гена очень много) Есть несколько способов нормализации данных: RPM, RPKM и TPM. /
RPKM (Reads per kilo base per million mapped reads) - число чтений для генов умножается на 10^9 и делится на длину гена и на число ридов для образца.
TMP (Transcripts per million) - число чтений для генов умножается на 10^6 и делится на длину гена, а потом происходит нормализация на глубину последовательности.
RPM (Reads per million) - число чтений для генов умножается на 10^6 и делитсяна число ридов для образца.
Первые два нам не подходят, так как длины генов нам не даны, поэтому воспользуемся RPM.
# Скрины heatmap мой и из статьи

![image](https://github.com/prayforanya/hse23_hw5/blob/main/images/experiment.png)
![image](https://github.com/prayforanya/hse23_hw5/blob/main/images/my.png)

RPM оказался не так плох и результаты получились очень похожи на те, что в статье.
# Визуализация данных по экспрессии на основе UMAP и PCA
![image](https://github.com/prayforanya/hse23_hw5/blob/main/images/pca.png)
![image](https://github.com/prayforanya/hse23_hw5/blob/main/images/umap.png)

PCA плохо справился с выделением подгрупп, UMAP лучше справляется с этой задачей. У PCA лучше всего получилось отделить подгруппу mTEC-I, а у UMAP - MTEC-IV.

# Графики бонусной части

![image](https://github.com/prayforanya/hse23_hw5/blob/main/images/markers.png)
![image](https://github.com/prayforanya/hse23_hw5/blob/main/images/all.png)
![image](https://github.com/prayforanya/hse23_hw5/blob/main/images/diff_mean.png)
![image](https://github.com/prayforanya/hse23_hw5/blob/main/images/by_groups.png)
