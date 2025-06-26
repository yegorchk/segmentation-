# Датасеты, использованные для сегментации дороги

| Датасет | Краткое описание | Ссылка |
|---------|------------------|--------|
| **Cityscapes** | 5 000 плотно размеченных уличных сцен (19 классов) в 50 городах Европы <br>Использовались пары `leftImg8bit` + `gtFine_labelIds` (классы *road* = 7, *sidewalk* = 8). | <https://www.cityscapes-dataset.com/> |
| **Crack & Pothole Segmentation** | 20 000 + изображений дорожного покрытия с Pixel-wise разметкой трещин и ям (4 класса). Брали только PNG-маски из папок `masks/` (класс *crack* / *pothole* → 3). | <https://datasets.towardsai.net/crack_pothole_segmentation> |

> **Примечание:**  
> * Для повторения эксперимента положите Cityscapes в  
>   `data/cityscapes/{images,masks}/…`  
>   и Crack&Pothole в  
>   `data/potholes/{images,masks}/…` (структура описана в `00_prepare_data.ipynb`).  
> * Скрипт конвертации json-масок Crack&Pothole → PNG находится в ячейке 3 фай­ла `00_prepare_data.ipynb`.
# Веса уже обученной модели лежат в Диске: https://drive.google.com/file/d/1qID8iqPw6ZocwSt-0gaZ3USHBBzXbOAg/view?usp=sharing
