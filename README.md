# Binary-Search-Tree-Projesi
[Ödev Linki](https://app.patika.dev/courses/veri-yapilari-ve-algoritmalar/binary-search-tree-proje)Binary Search Tree
# Proje-3
### [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] dizisinin Binary-Search-Tree aþamalarýný yazýnýz.
##### Ýkili arama aðacý, her düðümün solundaki koldan ulaþýlabilecek bütün verilerin düðümün deðerinden küçük, sað kolundan ulaþýlabilecek verilerin deðerinin o düðümün deðerinden büyük olmasýný þart koþar.

|     Açýklama    |  |  |  |
|--               |- |- |- |
|**root=7**       |  | 7|  |



**5 sayýsý 7'den küçük olduðunda 7'nin soluna ekledik**
|   Açýklama  |     |  |  |
|--           |-    |- |- |
|             |     |  | 7|  
|             |     | /|  | 
|**5 ekledik**|**5**|  |  | 


**1 sayýsý 5'ten ve 7'den küçük olduðunda 7 ve 5'in soluna ekledik** 
|     Açýklama  |     |  |  |  |  |
|             --|--   |--|- |- |- |
|               |     |  |  |  | 7|  
|               |     |  |  | /|  | 
|               |     |  | 5|  |  |  
|               |     | /|  |  |  | 
|**1 ekledik**  |**1**|  |  |  |  |

**8 sayýsý 7'den büyük olduðunda 7'nin saðýna ekledik** 
| Açýklama      |  |  |  |  |  |  |     |
|--             |--|--|- |- |- |- |-    |
|               |  |  |  |  | 7|  |     |  
|               |  |  |  | /|  |\ |     | 
|**8 ekledik**  |  |  | 5|  |  |  |**8**| 
|               |  | /|  |  |  |  |     | 
|               | 1|  |  |  |  |  |     |

**3 sayýsý  7'den ve 5'ten küçük  olduðunda 5'in soluna, 1'den büyük olduðunda 1'in saðýna ekledik**  
|  Açýklama     |  |  |     |  |  |  |  |
|--             |--|--|-    |- |- |- |- |
|               |  |  |     |  | 7|  |  |  
|               |  |  |     | /|  |\ |  | 
|               |  |  | 5   |  |  |  |8 | 
|               |  | /|     |  |  |  |  | 
|               | 1|  |     |  |  |  |  |
|               |  |\ |     |  |  |  |  |
|**3 ekledik**  |  |  |**3**|  |  |  |  |

**6 sayýsý 7'den küçük  olduðunda 7'nin soluna, 5'ten büyük olduðunda 5'in saðýna ekledik**  
| Açýklama      |  |  |  |  |     |  |  |
|--             |--|--|- |- |-    |- |- |
|               |  |  |  |  | 7   |  |  |  
|               |  |  |  | /|     |\ |  | 
|               |  |  | 5|  |     |  |8 | 
|               |  | /|  |\ |     |  |  | 
| **6 ekledik** | 1|  |  |  |**6**|  |  |
|               |  |\ |  |  |     |  |  |
|               |  |  | 3|  |     |  |  |

**0 sayýsý  7'den, 5'ten ve 1'den küçük  olduðunda 1'in soluna ekledik**  
| Açýklama       |     |  |  |  |  |  |  |  |  |
|--              |--   |--|- |- |- |- |- |- |- |
|                |     |  |  |  |  |  | 7|  |  |  
|                |     |  |  |  |  | /|  |\ |  | 
|                |     |  |  |  | 5|  |  |  |8 | 
|                |     |  |  | /|  |\ |  |  |  |
|                |     |  | 1|  |  |  |6 |  |  |
|                |     | /|  |\ |  |  |  |  |  |
| **0 ekledik**  |**0**|  |  |  | 3|  |  |  |  |

**9 sayýsý  7'den ve 8'den büyük olduðunda  8'in saðýna ekledik**  
| Açýklama     |  |  |  |  |  |  |  |  |  |  |     |
|--            |--|--|- |- |- |- |- |- |- |- |-    |
|              |  |  |  |  |  |  | 7|  |  |  |     |  
|              |  |  |  |  |  | /|  |\ |  |  |     | 
|              |  |  |  |  | 5|  |  |  |8 |  |     | 
|              |  |  |  | /|  |\ |  |  |  |\ |     | 
| **9 ekledik**|  |  | 1|  |  |  |6 |  |  |  |**9**|
|              |  | /|  |\ |  |  |  |  |  |  |     |
|              | 0|  |  |  | 3|  |  |  |  |  |     |


**4 sayýsý  7'den ve 5'ten küçük olduðunda 5'in soluna, 1'den ve 3'ten büyük olduðunda 3'ün saðýna ekledik** 
| Açýklama    |  |  |  |  |  |  |     |  |  |  |  |
|--           |--|--|- |- |- |- |-    |- |- |- |- |
|             |  |  |  |  |  |  | 7   |  |  |  |  |  
|             |  |  |  |  |  | /|     |\ |  |  |  | 
|             |  |  |  |  | 5|  |     |  |8 |  |  | 
|             |  |  |  | /|  |\ |     |  |  |\ |  |
|             |  |  | 1|  |  |  |6    |  |  |  | 9|
|             |  | /|  |\ |  |  |     |  |  |  |  |
|             | 0|  |  |  | 3|  |     |  |  |  |  |
|             |  |  |  |  |  |\ |     |  |  |  |  |
|**4 ekledik**|  |  |  |  |  |  |**4**|  |  |  |  |

**2 sayýsý  7'den ve 5'ten küçük olduðunda 5'in soluna, 1'den büyük olduðunda 1'in saðýna ve 3'ten küçük olduðunda 3'ün soluna ekledik** 
| Açýklama    |  |  |     |  |  |  |  |  |  |  |  |
|--           |--|--|-    |- |- |- |- |- |- |- |- |
|             |  |  |     |  |  |  | 7|  |  |  |  |  
|             |  |  |     |  |  | /|  |\ |  |  |  | 
|             |  |  |     |  | 5|  |  |  |8 |  |  | 
|             |  |  |     | /|  |\ |  |  |  |\ |  | 
|             |  |  | 1   |  |  |  |6 |  |  |  | 9|
|             |  | /|     |\ |  |  |  |  |  |  |  |
|             | 0|  |     |  | 3|  |  |  |  |  |  |
|             |  |  |     | /|  |\ |  |  |  |  |  |
|**2 ekledik**|  |  |**2**|  |  |  |4 |  |  |  |  |

