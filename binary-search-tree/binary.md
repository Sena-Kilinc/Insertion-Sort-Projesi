# Binary Search Tree

## [7, 5, 1, 8, 3, 6, 0, 9, 4, 2]

### Binary Search Tree aşamalarını yazınız.

**İlk önce root belirliyoruz. Diyelim ki 7 olsun.**
| | | |
| --- | --- | --- |
| | 7 | |

**5 sayısı 7'den küçük olduğu için sol tarafına eklenir.**
| | | |
|- |- |- |
| | | 7|  
| | /| |
|**5**| | |

**1 sayısı 5'ten ve 7'den küçük olduğu için 7 ve 5'in soluna eklenir**
| | | | | |
|-- |--|- |- |- |
| | | | | 7|  
| | | | /| |
| | | 5| | |  
| | /| | | |
|**1**| | | | |

**8 sayısı 7'den büyük olduğu için 7'nin sağına eklenir**
| | | | | | | |
|--|--|- |- |- |- |- |
| | | | | 7| | |  
| | | | /| |\ | |
| | | 5| | | |**8**|
| | /| | | | | |
| 1| | | | | | |

**Bu şekilde devam ediyor.**
| | | | | | | |
|--|--|- |- |- |- |- |
| | | | | 7| | |  
| | | | /| |\ | |
| | | 5 | | | |8 |
| | /| | | | | |
| 1| | | | | | |
| |\ | | | | | |
| | |**3**| | | | |

|     |     |     |     |       |     |     |
| --- | --- | --- | --- | ----- | --- | --- |
|     |     |     |     | 7     |     |     |
|     |     |     | /   |       | \   |     |
|     |     | 5   |     |       |     | 8   |
|     | /   |     | \   |       |     |     |
| 1   |     |     |     | **6** |     |     |
|     | \   |     |     |       |     |     |
|     |     | 3   |     |       |     |     |

|       |     |     |     |     |     |     |     |     |
| ----- | --- | --- | --- | --- | --- | --- | --- | --- |
|       |     |     |     |     |     | 7   |     |     |
|       |     |     |     |     | /   |     | \   |     |
|       |     |     |     | 5   |     |     |     | 8   |
|       |     |     | /   |     | \   |     |     |     |
|       |     | 1   |     |     |     | 6   |     |     |
|       | /   |     | \   |     |     |     |     |     |
| **0** |     |     |     | 3   |     |     |     |     |

|     |     |     |     |     |     |     |     |     |     |       |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | ----- |
|     |     |     |     |     |     | 7   |     |     |     |       |
|     |     |     |     |     | /   |     | \   |     |     |       |
|     |     |     |     | 5   |     |     |     | 8   |     |       |
|     |     |     | /   |     | \   |     |     |     | \   |       |
|     |     | 1   |     |     |     | 6   |     |     |     | **9** |
|     | /   |     | \   |     |     |     |     |     |     |       |
| 0   |     |     |     | 3   |     |     |     |     |     |       |

|     |     |     |     |     |     |       |     |     |     |     |
| --- | --- | --- | --- | --- | --- | ----- | --- | --- | --- | --- |
|     |     |     |     |     |     | 7     |     |     |     |     |
|     |     |     |     |     | /   |       | \   |     |     |     |
|     |     |     |     | 5   |     |       |     | 8   |     |     |
|     |     |     | /   |     | \   |       |     |     | \   |     |
|     |     | 1   |     |     |     | 6     |     |     |     | 9   |
|     | /   |     | \   |     |     |       |     |     |     |     |
| 0   |     |     |     | 3   |     |       |     |     |     |     |
|     |     |     |     |     | \   |       |     |     |     |     |
|     |     |     |     |     |     | **4** |     |     |     |     |

|     |     |       |     |     |     |     |     |     |     |     |
| --- | --- | ----- | --- | --- | --- | --- | --- | --- | --- | --- |
|     |     |       |     |     |     | 7   |     |     |     |     |
|     |     |       |     |     | /   |     | \   |     |     |     |
|     |     |       |     | 5   |     |     |     | 8   |     |     |
|     |     |       | /   |     | \   |     |     |     | \   |     |
|     |     | 1     |     |     |     | 6   |     |     |     | 9   |
|     | /   |       | \   |     |     |     |     |     |     |     |
| 0   |     |       |     | 3   |     |     |     |     |     |     |
|     |     |       | /   |     | \   |     |     |     |     |     |
|     |     | **2** |     |     |     | 4   |     |     |     |     |