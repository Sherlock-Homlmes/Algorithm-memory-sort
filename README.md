# Algorithm-memory-sort
### **Created: 2-5-2022**
### - **Memorysort là 1 thuật toán _đơn giản, đặc biệt hữu hiệu với việc sắp xếp những số không quá lớn trong 1 mảng gồm rất nhiều phần tử._**
### - **Thuật toán sử dụng RAM để có thể lưu trữ, sắp xếp các phần tử**

# Ưu điểm:
### Memorysort mang đến 1 hiệu năng đáng kinh ngạc so với quicksort(thuật toán được cho là nhanh nhất trong việc sắp xếp hiện nay) trong những trường hợp nhất định. Và vượt xa quicksort(trong Python) nếu không sử dụng library bên ngoài(numpy) để sắp xếp

# Nhược điểm:
### - Hiệu năng khi sắp xếp 1 mảng có số lớn giảm đáng kể
### - Tràn RAM nếu sắp xếp 1 số quá lớn

# Độ phức tạp:
###  **O(2n)**
 
# Thuật toán:
```
def basic_memory_sort(array):
 print("basic memory sort")
 result = []
 number_sort = len(array)
 number_limit = max(array)

 count_list  = [0] * (number_limit+1)
 for i in range(number_sort):
   count_list[array[i]] += 1

 for i in range(number_limit):
   if count_list[i] != 0:
    for x in range(count_list[i]):
      result.append(i)
      
 return result
```

# Khảo sát thời gian chạy:

# Cải tiến cho Python:

 

